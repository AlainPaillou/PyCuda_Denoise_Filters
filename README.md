# PyCuda_Denoise_Filters
Some PyCuda routines to denoise pictures

Thoses sample programs perform denoise filters applied to images (monochrome or colour). The programs compare OpenCV routines and PyCuda routines.

OpenCV is also used to load and save the test pictures. That is to say pictures format is 3D array (0 to 255 range value) for colour pictures and 1D array for mono pictures.

The base algorythms are provided by Nvidia (CUDA SDK samples).

initial CUDA examples use Tex2D to perform denoise.

I had to change CUDA examples to avoid Tex2D use in order to simply use my pictures (3D arrays with 0-255 range values) withou using texture functions.

Those programs where tested with Nvidia Jetson Nano (L4T OS).


**** UPDATE August 1st 2019

Code has been changed to avoid border effect error (array index out of range)

License statement :
Those programs re free of use for any kind of use.
