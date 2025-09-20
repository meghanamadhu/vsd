Week0 Tool Installation Guidelines
Setting up of Yosys tool  

```sudo apt-get update
git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt install make
sudo apt-get install build-essential clang bison flex \
libreadline-dev gawk tcl-dev libffi-dev git \
graphviz xdot pkg-config python3 libboost-system-dev \
libboost-python-dev libboost-filesystem-dev zlib1g-dev
make config-gcc
make
sudo make install


<img width="883" height="556" alt="Openlane" src="https://github.com/user-attachments/assets/185fa829-67f7-450f-bac0-ce6b8049b6e9" />




