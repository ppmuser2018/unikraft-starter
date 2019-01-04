# unikraft-starter
Repository for evaluation of [Unikraft](https://www.xenproject.org/developers/teams/unikraft.html).

## Setup
[CentOS](https://www.centos.org/) enviroment is required. 
#### 1.Install GNU make 4.1
```
cd /tmp
wget http://ftp.gnu.org/gnu/make/make-4.1.tar.gz
tar xvf make-4.1.tar.gz
cd make-4.1/
./configure
make
sudo make install
cd ..
rm -rf make-4.1.tar.gz make-4.1
export PATH=$PATH:/usr/local/bin/make
```
You can make it your default make by prefixing /usr/local/bin to your $PATH variable in your shell startup file; for instance, in .bashrc if you use the bash shell.

#### 2.Install ncurses
```
yum install -y ncurses-devel
```

#### 3.Get modules
```
git clone --recurse-submodules https://github.com/ppmuser2018/unikraft-starter.git
```

## Build helloworld by Unikraft
```
cd ./unikraft-starter/apps/helloworld
make menuconfig
make
```

## Run helloworld
```
./build/helloworld_linuxu-x86_64
```
