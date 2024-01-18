# NS-3 

## Table of Contents
1. [NS-3 Overview](#NS-3-Overview)
2. [Install NS-3](#Install-NS-3)
   - [Dependency](#Dependency)
   - [Install](#Install)
4. [Topology](#Topology)
5. [Project Execution Steps](#Project-Execution-Steps)
6. [Result](#Result)


## NS-3 Overview
- **NS-3:**
  - Discrete-event network simulator for Internet systems.
  - Designed for research and educational use.
  - Free, open-source software, licensed under the GNU GPLv2 license.
  - Maintained by a worldwide community.
  - Used to evaluate the performance of a network protocol design.

## Install-NS-3

### Dependency
[Reference1](https://karimmd.github.io/post/tutorial/ns3_installation/)
[Reference2](https://hackmd.io/@tomorrow3h/ns3)
#### Make sure that you are on the Home Directory
``` shellscript=
cd ~
```
#### Update the Ubuntu Repo and Existing Applications
``` shellscript=
sudo apt update && sudo apt -y upgrade
```
#### Install Core Dependencies for Build and Compilation
``` shellscript=
sudo apt install build-essential libsqlite3-dev libboost-all-dev libssl-dev git python3-setuptools castxml
```
#### Install Dependencies for NS-3 Python bindings
``` shellscript=
sudo apt install gir1.2-goocanvas-2.0 gir1.2-gtk-3.0 libgirepository1.0-dev python3-dev python3-gi python3-gi-cairo python3-pip python3-pygraphviz python3-pygccxml
```
#### Install Dependencies for NS-3
``` shellscript=
sudo apt install g++ pkg-config sqlite3 qt5-default mercurial ipython3 openmpi-bin openmpi-common openmpi-doc libopenmpi-dev autoconf cvs bzr unrar gdb valgrind uncrustify doxygen graphviz imagemagick python3-sphinx dia tcpdump libxml2 libxml2-dev cmake libc6-dev libc6-dev-i386 libclang-dev llvm-dev automake
sudo apt-get install qtbase5-dev qtchooser qt5-qmake qtbase5-dev-tools
sudo apt-get install vtun lxc
```

### Install
[ns-3 tutorial](https://www.nsnam.org/docs/tutorial/html/getting-started.html#downloading-ns-3-using-git)
#### Downloading ns-3 using Git
``` shellscript=
mkdir workspace
cd workspace
git clone https://gitlab.com/nsnam/ns-3-allinone.git
cd ns-3-allinone
```
#### README
``` shellscript=
./download.py
./build.py --enable-examples --enable-tests
```

## Topology
![Topology](https://github.com/Lewis-panda/Network-Simulator-with-Ns-3/assets/116704255/390b032d-23c1-4861-97bc-c4170c6db24b)



## Project Execution Steps
Follow these steps to execute the NS-3 project:
```bash
$ cp simulator.cc /workspace/ns-3-allinone/ns-3-dev
$ cd /workspace/ns-3-allinone/ns-3-dev
$ ./nd3 run scratch/simulator
```

## Result
![Result](https://github.com/Lewis-panda/Network-Simulator-with-Ns-3/assets/116704255/6d4e56a2-9c8e-4c2d-878d-d437bc0268f9)




