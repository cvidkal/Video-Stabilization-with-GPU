# Video-Stabilization-with-GPU
This is a Video stabilization program based on OpenCV videostab module

It  use OpenCL or CUDA to accelerate the stabilization algorithm.

All the useful defines are defined in define.h, you can change the defines to swtich the options.

It can only build on OpenCV 2.x.


## How To Build

1. mkdir build
2. cmake ..
3. make -j4