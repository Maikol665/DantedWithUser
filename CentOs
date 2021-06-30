#!/bin/bash
#
#   Mining Monero Script
#   -- Author:      Miikee

#
sudo yum install -y wget screen epel-release
#
sudo yum -y install centos-release-scl
#
sudo yum -y install devtoolset-8-gcc*
#
scl enable devtoolset-8 bash
#
#
#
sudo yum install -y git make cmake gcc gcc-c++ libstdc++-static libuv-static hwloc-devel openssl-devel
#
git clone https://github.com/xmrig/xmrig.git
#
mkdir xmrig/build && cd xmrig/build
#
cmake ..
#
make -j$(nproc)
