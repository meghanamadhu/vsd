Week0 Tool Installation Guidelines
```Setting up of Yosys tool  

sudo apt-get update
git clone https://github.com/YosysHQ/yosys.git```
cd yosys
sudo apt install make
sudo apt-get install build-essential clang bison flex \
libreadline-dev gawk tcl-dev libffi-dev git \
graphviz xdot pkg-config python3 libboost-system-dev \
libboost-python-dev libboost-filesystem-dev zlib1g-dev
make config-gcc
make
sudo make install
The image of installed tools
Iverilog Installation
sudo apt-get update
sudo apt-get install iverilog
![yosys](https://github.com/user-attachments/assets/f130d777-c6ff-4884-803f-40cb0ee4c332)


gtkwave
sudo apt-get update
sudo apt install gtkwave

ngspice
tar -zxvf ngspice-37.tar.gz
cd ngspice-37
mkdir release
cd release
../configure --with-x --with-readline=yes --disable-debug
make
sudo make install
<img width="890" height="557" alt="ngspice" src="https://github.com/user-attachments/assets/774755bb-f64b-4d99-8173-fa9913857fd3" />

Magic Installation
sudo apt-get install m4
sudo apt-get install tcsh
sudo apt-get install csh
sudo apt-get install libx11-dev
sudo apt-get install tcl-dev tk-dev
sudo apt-get install libcairo2-dev
sudo apt-get install mesa-common-dev libglu1-mesa-dev
sudo apt-get install libncurses-dev
git clone https://github.com/RTimothyEdwards/magic
cd magic
./configure
make
make install
<img width="905" height="558" alt="magic" src="https://github.com/user-attachments/assets/17ee40dd-5bf4-4929-88ee-b36691046864" />



Openlane
sudo apt-get update
sudo apt-get upgrade
sudo apt install -y build-essential python3 python3-venv python3-pip make git
sudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o
/usr/share/keyrings/docker-archive-keyring.gpg
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg]
https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee
/etc/apt/sources.list.d/docker.list > /dev/null
sudo apt update
sudo apt install docker-ce docker-ce-cli containerd.io
sudo docker run hello-world
sudo groupadd docker
sudo usermod -aG docker $USER
sudo reboot
cd $HOME
git clone https://github.com/The-OpenROAD-Project/OpenLane
cd OpenLane
make
make test
<img width="883" height="556" alt="Openlane" src="https://github.com/user-attachments/assets/9c0c3c92-4925-4aa7-af17-107b650ee78f" />











