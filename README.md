# Hello C++ in Resin.io

This is a very simple project that is an example of how to run C++ code on a device that is supported by [Resin.io](http://resin.io).

### Note for Raspberry pi 1
If the device you are planning to use is a raspberry pi 1 you will have to modify Dockerfile.template in order to use the application.
```
FROM resin/%%RESIN_MACHINE_NAME%%-debian
```
To
```
FROM resin/%%RESIN_MACHINE_NAME%%-raspbian
```