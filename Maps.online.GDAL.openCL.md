---
id: aDv7G32lC3EIeLupomXgy
title: openCL
desc: ''
updated: 1642633914706
created: 1642633366020
---
https://gis.stackexchange.com/questions/274896/gdal-usage-of-gpu-with-windows
-multi -wo "USE_OPENCL=TRUE"

https://gdal.org/gdal.pdf
GDAL Documentation
OpenCL
The OpenCL library may be used to accelerate warping computations, typically with a GPU.
Note: It is disabled by default even when detected, since the current OpenCL warping implementation lags behind
the generic implementation.
OpenCL_INCLUDE_DIR
Path to an include directory with the CL/cl.h header file.
OpenCL_LIBRARY
Path to a shared or static library file.
GDAL_USE_OPENCL=ON/OFF
Control whether to use OPENCL. Defaults to OFF when OPENCL is found.
