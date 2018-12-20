# Install Opensplice 

For bash script 

* Tested on Ubuntu 16.04 
* GCC 5.4 (Check using gcc --version)

```
$ ./installopensplicelinuxgcc54
```



:warning: Opensplice tutorial compiling problem

1. Edit `HDE/x86_64.linux/custom_lib/Makefile.Build_DCPS_ISO_Cpp_Lib` in Opensplice directory and add `-std=c++0x` to the `CPPFLAGS`
2. Recompile `make -f Makefile.Build_DCPS_ISO_Cpp_Lib` 



Problem: Library included was compiled using Boost shared pointers instead of C++11