# unikraft-test
https://www.xenproject.org/developers/teams/unikraft.html

## Setup
centos enviroment is required.
install make ver 4.0.
```
git clone https://github.com/ppmuser2018/unikraft-starter.git
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
