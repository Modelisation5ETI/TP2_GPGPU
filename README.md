

##*Generic Programming on GPU*

-----
**CMake Build instructions**

-----
  - Out-of-source build :
 ```
git clone git@github.com:Modelisation5ETI/TP2_GPGPU.git && \
mkdir TP2_GPGPU-build && cd TP2_GPGPU-build  && \
cmake ../TP2_GPGPU  && \
make -j
 
 ```
  - QtCreator :
 ```
git clone git@github.com:Modelisation5ETI/TP2_GPGPU.git  && \
mkdir TP2_GPGPU-build && cd TP2_GPGPU-build  && \
qtcreator ../TP2_GPGPU
 
 ```
  *Then configure project using QtCreator API* : 
   - *Set the build directory to TP2_GPGPU-build/*
   - *Run CMake and build project*


-----
**Implementation**

-----

 - ### Transform Feedback
 <img src="./Screenshots/TF_particle.png" alt="FBO" width="200" height="200" />

 ```
 ./TransformFeedback_
 ```
 
 This program uses Transform Feedback Buffers to animate a particle system.
 
 Use arrows to move the point where particles converge.
 
 - ### Image simple
 <img src="./Screenshots/contour.png" alt="SobelFilter" width="200" height="100" />
 <img src="./Screenshots/blur.png" alt="Blur" width="200" height="100" />
 <img src="./Screenshots/sat1.png" alt="Saturation" width="200" height="100" />
 <img src="./Screenshots/threshold.png" alt="Threshold" width="200" height="100" />
 
 ```
 ./ImageSimple_
 ``` 
 Process image filters on GPU.
 
 Use [0,1,2,3,4] keys to process different filters.
 
 Use arrow UP or DOWN to change the filter parameter.

 - ### Frame Buffer Object
 <img src="./Screenshots/FBO_tv.png" alt="FBO" width="200" height="150" />

 ```
 ./FrameBufferObject_
 ```
 Render a scene into a frame buffer object (FBO) and use its texture to render another scene in the current buffer.
 
 Use arrow LEFT or RIGHT to interact with the 'FBO' scene.
