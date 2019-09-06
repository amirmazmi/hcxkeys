hcxkeys
==============

Small set of tools to generate plainmasterkeys (rainbowtables) and hashes
for the use with latest hashcat and latest John the Ripper.


Brief description
--------------

Multiple stand-alone binaries.

All of these utils are designed to execute only one specific function.

Read this post: hcxtools - solution for capturing wlan traffic and conversion to hashcat formats (https://hashcat.net/forum/thread-6661.html)


Detailed description
--------------

| Tool           | Description                                                                                          |
| -------------- | ---------------------------------------------------------------------------------------------------- |
| wlangenpmk     | Generates plainmasterkeys (CPU) from essid and password for use with hashcat hash-mode 2501          |
| wlangenpmkocl  | Generates plainmasterkeys (GPU) from essid and password for use with hashcat hash-mode 2501          |
| pwhash         | Generate hash of a word by using a given charset                                                     |

To list available platforms  
```wlangenpmkocl -l```

Otherwise install clinfo  
```sudo apt install clinfo```

  
  
  
Compile
--------------

Simply run:
```
make
make install (as super user)
```


Requirements
--------------

* Linux (recommended Arch, but other distros should work, too)
* OpenCL and OpenCL Headers installed
* libopenssl and openssl-dev installed
* librt and librt-dev installed (should be installed by default)


For Ubuntu  
```sudo apt install ocl-icd-* opencl-headers```  




Notice
--------------

Most output files will be appended to existing files.


