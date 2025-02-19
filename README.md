# canfd_networking

## Description
A simple kernel module with a user-space application.

## Project Structure
```
canfd_networking/
├── kernel_module/
│   ├── src/
│   │   └── canfd_networking.c
│   ├── include/
│   │   └── canfd_networking.h
│   └── Makefile
└── application/
    ├── main.c
    └── CMakeLists.txt
```

## Build

### Kernel Module
```bash
cd canfd_networking/kernel_module
make
```

### Application
```bash
cd canfd_networking/application
cmake .
make
```

## Usage

### Kernel Module
```bash
sudo insmod canfd_networking/kernel_module/canfd_networking.ko
# Do something with the module
sudo rmmod canfd_networking
```

### Application
```bash
cd canfd_networking/application
./test_app
```

## License
GPL
