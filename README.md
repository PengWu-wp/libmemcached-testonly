# libmemcached-testonly

Wanted to use memaslap tool in libmemcached, but official program have some issues on Ubuntu 20.04. So have this repo for fixing.

Based on libmemcached-v1.0.18. Fixed some compatibility issues. 

## Build step

```bash
tar -zxf libmemcached-wp.tar.gz
cd libmemcached-1.0.18
./configure --enable-memaslap LDFLAGS=-lpthread
make
```

> Note that libmemcached-wp-1.2.tar.gz is for my own purpose. Core code modified.
