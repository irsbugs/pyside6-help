# pyside6-help

PySide6 is a Python wrapper for Qt https://www.qt.io/ Version 6 software. Qt is cross-platform software for creating graphical user interfaces written in C++. https://wiki.qt.io/Qt_for_Python

pyside6-assistant.py is a python program designed to provide help when writing PySide6 programs.

Where the examples reside... https://code.qt.io/cgit/pyside/pyside-setup.git/tree/


```
PySide6 Installation to support Qt6 13 sep 2022

HomePage: https://wiki.qt.io/Qt_for_Python

PyPI: https://pypi.org/project/PySide6/



    Detected that PyQt6 modules are not installed.
    
    To install PySide6 in a virtual environment on a Linux system:
    
ian@hp:~$ python3 -m venv venv-pyside6
    
ian@hp:~$ source venv-pyside6/bin/activate

(venv-pyside6) ian@hp:~$ cd venv-pyside6/  
  
(venv-pyside6) ian@hp:~/venv-pyside6$ python -m pip install -U pip setuptools wheel 
 
(venv-pyside6) ian@hp:~/venv-pyside6$ pip install PySide6 

    
# For a list of modules that are installed:
(venv-pyside6) ian@hp:~/venv-pyside6$ ls ./lib/python3.10/site-packages/PySide6/include/ -1

Total: 46 Modules.


# Check program:
(venv-pyside6) ian@hp:~/venv-pyside6$ python
Python 3.10.4 (main, Jun 29 2022, 12:14:53) [GCC 11.2.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import PySide6
>>> PySide6.__version__
'6.3.2'
>>> 

(venv-pyside6) ian@hp:~/venv-pyside6$ cd ..
(venv-pyside6) ian@hp:~$ cd pyside6
(venv-pyside6) ian@hp:~/pyside6$ 


=====
    
ian@hp:~$ python3 -m venv venv-pyside6
   
ian@hp:~$ source venv-pyside6/bin/activate

(venv-pyside6) ian@hp:~$ cd venv-pyside6/

(venv-pyside6) ian@hp:~/venv-pyside6$ python -m pip install -U pip setuptools wheel
Requirement already satisfied: pip in ./lib/python3.10/site-packages (22.0.2)
Collecting pip
  Using cached pip-22.2.2-py3-none-any.whl (2.0 MB)
Requirement already satisfied: setuptools in ./lib/python3.10/site-packages (59.6.0)
Collecting setuptools
  Using cached setuptools-65.3.0-py3-none-any.whl (1.2 MB)
Collecting wheel
  Using cached wheel-0.37.1-py2.py3-none-any.whl (35 kB)
Installing collected packages: wheel, setuptools, pip
  Attempting uninstall: setuptools
    Found existing installation: setuptools 59.6.0
    Uninstalling setuptools-59.6.0:
      Successfully uninstalled setuptools-59.6.0
  Attempting uninstall: pip
    Found existing installation: pip 22.0.2
    Uninstalling pip-22.0.2:
      Successfully uninstalled pip-22.0.2
Successfully installed pip-22.2.2 setuptools-65.3.0 wheel-0.37.1
(venv-pyside6) ian@hp:~/venv-pyside6$ 

=====

(venv-pyside6) ian@hp:~/venv-pyside6$ pip install PySide6
Collecting PySide6
  Downloading PySide6-6.3.2-cp36-abi3-manylinux_2_28_x86_64.whl (65 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 65.6/65.6 kB 778.0 kB/s eta 0:00:00
Collecting shiboken6==6.3.2
  Downloading shiboken6-6.3.2-cp36-abi3-manylinux_2_28_x86_64.whl (236 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 237.0/237.0 kB 1.4 MB/s eta 0:00:00
Collecting PySide6-Addons==6.3.2
  Downloading PySide6_Addons-6.3.2-cp36-abi3-manylinux_2_28_x86_64.whl (120.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 120.2/120.2 MB 1.1 MB/s eta 0:00:00
Collecting PySide6-Essentials==6.3.2
  Downloading PySide6_Essentials-6.3.2-cp36-abi3-manylinux_2_28_x86_64.whl (76.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 76.3/76.3 MB 1.0 MB/s eta 0:00:00
Installing collected packages: shiboken6, PySide6-Essentials, PySide6-Addons, PySide6
Successfully installed PySide6-6.3.2 PySide6-Addons-6.3.2 PySide6-Essentials-6.3.2 shiboken6-6.3.2
(venv-pyside6) ian@hp:~/venv-pyside6$ 

=====

Dependencies

PySide6 versions following 6.0 use a C++ parser based on Clang. The Clang library (C-bindings), version 13.0 or higher is required for building. Prebuilt versions of it can be downloaded from download.qt.io.

After unpacking the archive, set the environment variable LLVM_INSTALL_DIR to point to the folder containing the include and lib directories of Clang:

7z x .../libclang-release_100-linux-Rhel7.2-gcc5.3-x86_64-clazy.7z
export LLVM_INSTALL_DIR=$PWD/libclang


=====
https://download.qt.io/development_releases/prebuilt/libclang/

 Parent Directory	 	- 	 
testing/	30-Mar-2022 12:43 	- 	 
qt/	07-Jun-2022 09:14 	- 	 
md5sums.txt	28-Oct-2020 12:51 	5.1K 	Details
libclang-release_140-based-windows-vs2019_64.7z	03-Mar-2022 09:39 	449M 	Details
libclang-release_140-based-windows-mingw_64.7z	03-Mar-2022 09:38 	498M 	Details
libclang-release_140-based-windows-mingw_64-regular.7z	03-Mar-2022 09:39 	743M 	Details
libclang-release_140-based-md5.txt	03-Mar-2022 09:38 	520 	Details
libclang-release_140-based-macos-universal.7z	03-Mar-2022 09:38 	690M 	Details
libclang-release_140-based-linux-Ubuntu20.04-gcc9.3-x86_64.7z	03-Mar-2022 09:37 	479M 	Details
libclang-release_140-based-linux-Rhel8.2-gcc9.2-x86_64.7z	03-Mar-2022 09:37 	464M 	Details

https://download.qt.io/development_releases/prebuilt/libclang/libclang-release_140-based-linux-Ubuntu20.04-gcc9.3-x86_64.7z.mirrorlist
File information
File information

    Filename: Mirrors for libclang-release_140-based-linux-Ubuntu20.04-gcc9.3-x86_64.7z
    Filename: libclang-release_140-based-linux-Ubuntu20.04-gcc9.3-x86_64.7z
    Path: /development_releases/prebuilt/libclang/libclang-release_140-based-linux-Ubuntu20.04-gcc9.3-x86_64.7z
    Size: 479M (501830923 bytes)
    Last modified: Thu, 03 Mar 2022 07:37:37 GMT (Unix time: 1646293057)
    SHA-256 Hash: 7ffea68edcecce9f8a06b559afa36651664f79fbb8732c1c9f5db85dcb0d0a5c
    SHA-1 Hash: b43538251f059c2a8fc80fd71eabef98de4b0691
    MD5 Hash: e82b4f9ef315dc98786b7d937de1ef68
    BitTorrent Information Hash: 1c561d8171a8b0f67aadb8b41d0c65f9e5b8e05e

=====

(venv-pyside6) ian@hp:~/venv-pyside6$ ls ./lib/python3.10/site-packages/PySide6/include/ -1

Qt3DAnimation
Qt3DCore
Qt3DExtras
Qt3DInput
Qt3DLogic
Qt3DRender
QtBluetooth
QtCharts
QtConcurrent
QtCore
QtDataVisualization
QtDBus
QtDesigner
QtGui
QtHelp
QtMultimedia
QtMultimediaWidgets
QtNetwork
QtNetworkAuth
QtNfc
QtOpenGL
QtOpenGLWidgets
QtPositioning
QtPrintSupport
QtQml
QtQuick
QtQuick3D
QtQuickControls2
QtQuickWidgets
QtRemoteObjects
QtScxml
QtSensors
QtSerialPort
QtSql
QtStateMachine
QtSvg
QtSvgWidgets
QtTest
QtUiTools
QtWebChannel
QtWebEngineCore
QtWebEngineQuick
QtWebEngineWidgets
QtWebSockets
QtWidgets
QtXml

Total: 46 Modules.
=====

Add QScintilla

pip install QScintilla

(venv-pyside6) ian@hp:~$ pip install QScintilla
Collecting QScintilla
  Using cached QScintilla-2.13.3-cp37-abi3-manylinux1_x86_64.whl (2.8 MB)
Collecting PyQt5-sip<13,>=12.8
  Using cached PyQt5_sip-12.11.0-cp310-cp310-manylinux1_x86_64.whl (359 kB)
Collecting PyQt5>=5.15.4
  Using cached PyQt5-5.15.7-cp37-abi3-manylinux1_x86_64.whl (8.4 MB)
Collecting PyQt5-Qt5>=5.15.0
  Using cached PyQt5_Qt5-5.15.2-py3-none-manylinux2014_x86_64.whl (59.9 MB)
Installing collected packages: PyQt5-Qt5, PyQt5-sip, PyQt5, QScintilla
Successfully installed PyQt5-5.15.7 PyQt5-Qt5-5.15.2 PyQt5-sip-12.11.0 QScintilla-2.13.3
(venv-pyside6) ian@hp:~$ 

=====


(venv-pyside6) ian@hp:~$ pip install pygments
Collecting pygments
  Using cached Pygments-2.13.0-py3-none-any.whl (1.1 MB)
Installing collected packages: pygments
Successfully installed pygments-2.13.0
(venv-pyside6) ian@hp:~$ 

=====


```
