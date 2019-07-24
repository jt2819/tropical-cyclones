# tropical-cyclones

login as: egurop
Pre-authentication banner message from server:
|
| Unauthorised Access Is Prohibited [seldon.sp.ph.ic.ac.uk]
|
End of banner message from server
egurop@seldon.sp.ph.ic.ac.uk's password:
Last login: Wed Jul 24 20:34:55 2019 from spat-nas.sp.ph.ic.ac.uk

-------------------------------------------------
        Welcome to seldon.sp.ph.ic.ac.uk

     SPAT Physics, Imperial College London
          Authorised Users Only!

    This is an Oracle Enterprise Linux Server
(Single 2.1GHz Xeon E5-2620 v4, 8-CORES, 64GB RAM)
       LSI MEGARAID 9361-4i 1x RAID6
-------------------------------------------------

Filesystem                  Size  Used Avail Use% Mounted on
/dev/mapper/ol_seldon-root  160G   57G  104G  36% /
devtmpfs                     32G     0   32G   0% /dev
/dev/sda1                  1016M  206M  811M  21% /boot
/dev/sdb1                    15T   14T  1.3T  92% /disk1
egurop@seldon:~$ git clone git@cumulus.edgryspeerdt.com:csat
Cloning into 'csat'...
remote: Counting objects: 1715, done.
remote: Compressing objects: 100% (1685/1685), done.
remote: Total 1715 (delta 972), reused 0 (delta 0)
Receiving objects: 100% (1715/1715), 5.00 MiB | 6.34 MiB/s, done.
Resolving deltas: 100% (972/972), done.
egurop@seldon:~$ ls
csat
egurop@seldon:~$ pwd
/disk1/egurop
egurop@seldon:~$ ls /disk1/egurop/csat
env.yml  examples  lib  scripts
egurop@seldon:~$ export PYTHONPATH=$disk1/csat/lib:${PYTHONPATH}
egurop@seldon:~$ export PYTHONPATH=$disk1/egurop/csat/lib:${PYTHONPATH}
egurop@seldon:~$ ls
csat
egurop@seldon:~$ pwd
/disk1/egurop
egurop@seldon:~$ conda create -n py37 python=3.7
Fetching package metadata ...........
Solving package specifications: .

Package plan for installation in environment /disk1/egurop/.conda/envs/py37:

The following NEW packages will be INSTALLED:

    _libgcc_mutex:   0.1-main
    ca-certificates: 2019.5.15-0
    certifi:         2019.6.16-py37_0
    libedit:         3.1.20181209-hc058e9b_0
    libffi:          3.2.1-hd88cf55_4
    libgcc-ng:       9.1.0-hdf63c60_0
    libstdcxx-ng:    9.1.0-hdf63c60_0
    ncurses:         6.1-he6710b0_1
    openssl:         1.1.1c-h7b6447c_1
    pip:             19.1.1-py37_0
    python:          3.7.3-h0371630_0
    readline:        7.0-h7b6447c_5
    setuptools:      41.0.1-py37_0
    sqlite:          3.29.0-h7b6447c_0
    tk:              8.6.8-hbc83047_0
    wheel:           0.33.4-py37_0
    xz:              5.2.4-h14c3975_4
    zlib:            1.2.11-h7b6447c_3

Proceed ([y]/n)? y

_libgcc_mutex- 100% |#####################################################################| Time: 0:00:00   5.54 MB/s
ca-certificate 100% |#####################################################################| Time: 0:00:00  38.36 MB/s
libstdcxx-ng-9 100% |#####################################################################| Time: 0:00:00  16.28 MB/s
libgcc-ng-9.1. 100% |#####################################################################| Time: 0:00:00  40.76 MB/s
libffi-3.2.1-h 100% |#####################################################################| Time: 0:00:00  53.98 MB/s
ncurses-6.1-he 100% |#####################################################################| Time: 0:00:00  71.75 MB/s
openssl-1.1.1c 100% |#####################################################################| Time: 0:00:00  72.20 MB/s
xz-5.2.4-h14c3 100% |#####################################################################| Time: 0:00:00  68.55 MB/s
zlib-1.2.11-h7 100% |#####################################################################| Time: 0:00:00  68.46 MB/s
libedit-3.1.20 100% |#####################################################################| Time: 0:00:00  68.75 MB/s
readline-7.0-h 100% |#####################################################################| Time: 0:00:00  69.72 MB/s
tk-8.6.8-hbc83 100% |#####################################################################| Time: 0:00:00  74.57 MB/s
sqlite-3.29.0- 100% |#####################################################################| Time: 0:00:00  73.43 MB/s
python-3.7.3-h 100% |#####################################################################| Time: 0:00:00  70.51 MB/s
certifi-2019.6 100% |#####################################################################| Time: 0:00:00  60.98 MB/s
setuptools-41. 100% |#####################################################################| Time: 0:00:00  71.46 MB/s
wheel-0.33.4-p 100% |#####################################################################| Time: 0:00:00  52.24 MB/s
pip-19.1.1-py3 100% |#####################################################################| Time: 0:00:00  74.80 MB/s
#
# To activate this environment, use:
# > source activate py37
#
# To deactivate an active environment, use:
# > source deactivate
#

egurop@seldon:~$ source activate py37
(py37) egurop@seldon:~$ conda install numpy scipy matplotlib
Fetching package metadata ...........
Solving package specifications: .

Package plan for installation in environment /disk1/egurop/.conda/envs/py37:

The following NEW packages will be INSTALLED:

    blas:             1.0-mkl
    cycler:           0.10.0-py37_0
    dbus:             1.13.6-h746ee38_0
    expat:            2.2.6-he6710b0_0
    fontconfig:       2.13.0-h9420a91_0
    freetype:         2.9.1-h8a8886c_1
    glib:             2.56.2-hd408876_0
    gst-plugins-base: 1.14.0-hbbd80ab_1
    gstreamer:        1.14.0-hb453b48_1
    icu:              58.2-h9c2bf20_1
    intel-openmp:     2019.4-243
    jpeg:             9b-h024ee3a_2
    kiwisolver:       1.1.0-py37he6710b0_0
    libgfortran-ng:   7.3.0-hdf63c60_0
    libpng:           1.6.37-hbc83047_0
    libuuid:          1.0.3-h1bed415_2
    libxcb:           1.13-h1bed415_1
    libxml2:          2.9.9-hea5a465_1
    matplotlib:       3.1.0-py37h5429711_0
    mkl:              2019.4-243
    mkl-service:      2.0.2-py37h7b6447c_0
    mkl_fft:          1.0.12-py37ha843d7b_0
    mkl_random:       1.0.2-py37hd81dba3_0
    numpy:            1.16.4-py37h7e9f1db_0
    numpy-base:       1.16.4-py37hde5b4d6_0
    pcre:             8.43-he6710b0_0
    pyparsing:        2.4.0-py_0
    pyqt:             5.9.2-py37h05f1152_2
    python-dateutil:  2.8.0-py37_0
    pytz:             2019.1-py_0
    qt:               5.9.7-h5867ecd_1
    scipy:            1.3.0-py37h7c811a0_0
    sip:              4.19.8-py37hf484d3e_0
    six:              1.12.0-py37_0
    tornado:          6.0.3-py37h7b6447c_0

Proceed ([y]/n)? y

blas-1.0-mkl.t 100% |#####################################################################| Time: 0:00:00   9.88 MB/s
intel-openmp-2 100% |#####################################################################| Time: 0:00:00  58.42 MB/s
libgfortran-ng 100% |#####################################################################| Time: 0:00:00  30.11 MB/s
mkl-2019.4-243 100% |#####################################################################| Time: 0:00:02  73.82 MB/s
expat-2.2.6-he 100% |#####################################################################| Time: 0:00:00  65.35 MB/s
icu-58.2-h9c2b 100% |#####################################################################| Time: 0:00:00  73.03 MB/s
jpeg-9b-h024ee 100% |#####################################################################| Time: 0:00:00  70.66 MB/s
libuuid-1.0.3- 100% |#####################################################################| Time: 0:00:00  39.74 MB/s
libxcb-1.13-h1 100% |#####################################################################| Time: 0:00:00  67.96 MB/s
pcre-8.43-he67 100% |#####################################################################| Time: 0:00:00  66.31 MB/s
glib-2.56.2-hd 100% |#####################################################################| Time: 0:00:00  74.02 MB/s
libpng-1.6.37- 100% |#####################################################################| Time: 0:00:00  72.29 MB/s
libxml2-2.9.9- 100% |#####################################################################| Time: 0:00:00  40.16 MB/s
dbus-1.13.6-h7 100% |#####################################################################| Time: 0:00:00  72.31 MB/s
freetype-2.9.1 100% |#####################################################################| Time: 0:00:00  73.32 MB/s
gstreamer-1.14 100% |#####################################################################| Time: 0:00:00  73.18 MB/s
fontconfig-2.1 100% |#####################################################################| Time: 0:00:00  69.35 MB/s
gst-plugins-ba 100% |#####################################################################| Time: 0:00:00  73.53 MB/s
kiwisolver-1.1 100% |#####################################################################| Time: 0:00:00  55.30 MB/s
numpy-base-1.1 100% |#####################################################################| Time: 0:00:00  57.05 MB/s
pyparsing-2.4. 100% |#####################################################################| Time: 0:00:00  57.97 MB/s
pytz-2019.1-py 100% |#####################################################################| Time: 0:00:00  73.21 MB/s
qt-5.9.7-h5867 100% |#####################################################################| Time: 0:00:01  69.99 MB/s
sip-4.19.8-py3 100% |#####################################################################| Time: 0:00:00  66.49 MB/s
six-1.12.0-py3 100% |#####################################################################| Time: 0:00:00  40.97 MB/s
tornado-6.0.3- 100% |#####################################################################| Time: 0:00:00  71.11 MB/s
cycler-0.10.0- 100% |#####################################################################| Time: 0:00:00  35.39 MB/s
mkl_random-1.0 100% |#####################################################################| Time: 0:00:00  67.31 MB/s
pyqt-5.9.2-py3 100% |#####################################################################| Time: 0:00:00  71.40 MB/s
python-dateuti 100% |#####################################################################| Time: 0:00:00  69.97 MB/s
matplotlib-3.1 100% |#####################################################################| Time: 0:00:00  69.75 MB/s
mkl-service-2. 100% |#####################################################################| Time: 0:00:00  61.83 MB/s
mkl_fft-1.0.12 100% |#####################################################################| Time: 0:00:00  72.48 MB/s
numpy-1.16.4-p 100% |#####################################################################| Time: 0:00:00  52.52 MB/s
scipy-1.3.0-py 100% |#####################################################################| Time: 0:00:00  72.49 MB/s
(py37) egurop@seldon:~$ echo $PYTHONPATH
/egurop/csat/lib:/csat/lib:
(py37) egurop@seldon:~$ ~/.bashrc
-bash: /disk1/egurop/.bashrc: Permission denied
(py37) egurop@seldon:~$ echo $PYTHONPATH
/egurop/csat/lib:/csat/lib:
(py37) egurop@seldon:~$ ls csat/examples
readin_modis_subset.py
(py37) egurop@seldon:~$ pwd
/disk1/egurop
(py37) egurop@seldon:~$
