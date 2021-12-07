# Prebuilt binaries OpenCV C++ for Windows
##### Current stable build of gRPC v4.5.4
##### OpenCV [v4.5.4](https://github.com/grpc/grpc/releases/tag/v4.5.4) 

> They can be downloaded separately as zip archives from the  [releases](https://github.com/thommyho/Cpp-OpenCV-Windows-PreBuilts/releases) page


##### Releases

| Version | Commit | Debug | Release  | RelWithDebInfo | MSVC142 32Bit | MSVC142 64Bit | MSVC141 32 Bit | MSVC141 64 Bit | MSVC140 32 Bit | MSVC140 64 Bit | Example |
|---------|------------|-------|----------|----------------|---------------|---------------|----------------|----------------|----------------|----------------|---------|
| [4.5.4](https://github.com/thommyho/Cpp-OpenCV-Windows-PreBuilts/releases/tag/v4.5.4) | 4223495e6cd67011f86b8ecd9be1fa105018f3b1 | :ballot_box_with_check: | :ballot_box_with_check: | :ballot_box_with_check:              | :ballot_box_with_check:             | :ballot_box_with_check:             | :ballot_box_with_check:              | :ballot_box_with_check:              | :ballot_box_with_check:              | :ballot_box_with_check:              | :ballot_box_with_check:       |

HelloWorld-Example included. Tested with VS2015, VS2017 and VS2019 Enterprise and msvc140, msvc141, msvc142 (Win 10, SDK 10.X)

#### Information about Build system and Tools

| Operating System | SDK Version   |
|------------------|---------------|
| Windows 10 (x64) |  10.0.19044   |

| Build Tool       | Version        |
|------------------|----------------|
| cmake            | 3.20.0-rc1     |
| MSVC 140         | 19.0.24245.0   |
| MSVC 141         | 19.16.27045.0  |
| MSVC 142         | 19.29.30133.0  |

```console
General configuration for OpenCV 4.5.4 =====================================

  Version control:               4.5.4

  Platform:
    Timestamp:                   2021-12-07T09:53:22Z
    Host:                        Windows 10.0.19044 AMD64
    CMake:                       3.20.0-rc1    
    Configuration:               Debug Release MinSizeRel RelWithDebInfo

  CPU/HW features:
    Baseline:                    SSE SSE2
      requested:                 SSE2
    Dispatched code generation:  SSE4_1 SSE4_2 FP16 AVX
      requested:                 SSE4_1 SSE4_2 AVX FP16
      SSE4_1 (15 files):         + SSE3 SSSE3 SSE4_1
      SSE4_2 (1 files):          + SSE3 SSSE3 SSE4_1 POPCNT SSE4_2
      FP16 (0 files):            + SSE3 SSSE3 SSE4_1 POPCNT SSE4_2 FP16 AVX
      AVX (4 files):             + SSE3 SSSE3 SSE4_1 POPCNT SSE4_2 AVX

  C/C++:
    Built as dynamic libs?:      NO
    C++ standard:                11    
    ccache:                      NO
    Precompiled headers:         YES
    Extra dependencies:          wsock32 comctl32 gdi32 ole32 setupapi ws2_32
    3rdparty dependencies:       libprotobuf ade ittnotify libjpeg-turbo libpng libtiff libopenjp2 IlmImf zlib quirc ippiw ippicv

  OpenCV modules:
    To be built:                 aruco barcode bgsegm bioinspired calib3d ccalib core datasets dnn dnn_objdetect dnn_superres dpm face features2d flann fuzzy gapi hfs highgui img_hash imgcodecs imgproc intensity_transform line_descriptor mcc ml objdetect optflow phase_unwrapping photo plot quality rapid reg rgbd saliency shape stereo stitching structured_light superres surface_matching text tracking video videoio videostab wechat_qrcode xfeatures2d ximgproc xobjdetect xphoto
    Disabled:                    java_bindings_generator js_bindings_generator objc_bindings_generator python_bindings_generator python_tests world
    Disabled by dependency:      -
    Unavailable:                 alphamat cudaarithm cudabgsegm cudacodec cudafeatures2d cudafilters cudaimgproc cudalegacy cudaobjdetect cudaoptflow cudastereo cudawarping cudev cvv freetype hdf java julia matlab ovis python2 python3 sfm ts viz
    Applications:                apps
    Documentation:               NO
    Non-free algorithms:         NO

  Windows RT support:            NO

  GUI:                           WIN32UI
    Win32 UI:                    YES

  Media I/O: 
    ZLib:                        build (ver 1.2.11)
    JPEG:                        build-libjpeg-turbo (ver 2.1.0-62)
    PNG:                         build (ver 1.6.37)
    TIFF:                        build (ver 42 - 4.2.0)
    JPEG 2000:                   build (ver 2.4.0)
    OpenEXR:                     build (ver 2.3.0)
    HDR:                         YES
    SUNRASTER:                   YES
    PXM:                         YES
    PFM:                         YES

  Video I/O:
    DC1394:                      NO
    FFMPEG:                      YES (prebuilt binaries)
      avcodec:                   YES (58.134.100)
      avformat:                  YES (58.76.100)
      avutil:                    YES (56.70.100)
      swscale:                   YES (5.9.100)
      avresample:                YES (4.0.0)
    GStreamer:                   NO
    DirectShow:                  YES
    Media Foundation:            YES
      DXVA:                      YES

  Parallel framework:            Concurrency

  Trace:                         YES (with Intel ITT)

  Other third-party libraries:
    Intel IPP:                   2020.0.0 Gold [2020.0.0]
           at:                   C:/Projects/Jenkins/2/3/4/workspace/OpenCV-Build-Pkg/opencv/build_4.5.4_MSVC141_32/3rdparty/ippicv/ippicv_win/icv
    Intel IPP IW:                sources (2020.0.0)
              at:                C:/Projects/Jenkins/2/3/4/workspace/OpenCV-Build-Pkg/opencv/build_4.5.4_MSVC141_32/3rdparty/ippicv/ippicv_win/iw
    Lapack:                      NO
    Eigen:                       NO
    Custom HAL:                  NO
    Protobuf:                    build (3.5.1)

  OpenCL:                        YES (NVD3D11)
    Include path:                C:/Projects/Jenkins/2/3/4/workspace/OpenCV-Build-Pkg/opencv/3rdparty/include/opencl/1.2
    Link libraries:              Dynamic load  
-----------------------------------------------------------------

```

#### Directory Setup for using/testing the provided two basic examples

```console
.
+-- vs2015
|   +-- 0_HelperScripts
|       +-- 0_CopyFiles
|           +-- CopyFiles.vcxproj
|           +-- CopyFiles.vcxproj.filters
|           +-- CopyFiles.vcxproj
|   +-- 1_Print_Version
|       +-- Print_Version.vcxproj
|       +-- Print_Version.vcxproj.filter
|       +-- pch.h
|       +-- pch.cpp
|       +-- Print_Version.cpp
|   +-- 2_Image_Read_and_Display
|       +-- Image_Read_and_Display.vcxproj
|       +-- Image_Read_and_Display.vcxproj.filter
|       +-- pch.h
|       +-- pch.cpp
|       +-- Image_Read_and_Display.cpp
|   +-- OpenCV_PropertySheet
|       +-- OpenCV.props
|   +-- res
|       +-- starry_night.jpg
|   +-- Examples_vs2015.sln
+-- vs2017
|   +-- 0_HelperScripts
|       +-- 0_CopyFiles
|           +-- CopyFiles.vcxproj
|           +-- CopyFiles.vcxproj.filters
|           +-- CopyFiles.vcxproj
|   +-- 1_Print_Version
|       +-- Print_Version.vcxproj
|       +-- Print_Version.vcxproj.filter
|       +-- pch.h
|       +-- pch.cpp
|       +-- Print_Version.cpp
|   +-- 2_Image_Read_and_Display
|       +-- Image_Read_and_Display.vcxproj
|       +-- Image_Read_and_Display.vcxproj.filter
|       +-- pch.h
|       +-- pch.cpp
|       +-- Image_Read_and_Display.cpp
|   +-- OpenCV_PropertySheet
|       +-- OpenCV.props
|   +-- res
|       +-- starry_night.jpg
|   +-- Examples_vs2017.sln
+-- vs2019
|   +-- 0_HelperScripts
|       +-- 0_CopyFiles
|           +-- CopyFiles.vcxproj
|           +-- CopyFiles.vcxproj.filters
|           +-- CopyFiles.vcxproj
|   +-- 1_Print_Version
|       +-- Print_Version.vcxproj
|       +-- Print_Version.vcxproj.filter
|       +-- pch.h
|       +-- pch.cpp
|       +-- Print_Version.cpp
|   +-- 2_Image_Read_and_Display
|       +-- Image_Read_and_Display.vcxproj
|       +-- Image_Read_and_Display.vcxproj.filter
|       +-- pch.h
|       +-- pch.cpp
|       +-- Image_Read_and_Display.cpp
|   +-- OpenCV_PropertySheet
|       +-- OpenCV.props
|   +-- res
|       +-- starry_night.jpg
|   +-- Examples_vs2019.sln
# Extract the prebuilt bins and libs like this for your disired toolchain e.g.:
+-- MSVC142_64
|   +-- Debug
|       +-- bin
|       +-- etc
|       +-- include
|       +-- lib
|       +-- build_info.md
|       +-- LICENSE
|   +-- Release
|       +-- bin
|       +-- etc
|       +-- include
|       +-- lib
|       +-- build_info.md
|       +-- LICENSE
|   +-- RelWithDebInfo
|       +-- bin
|       +-- etc
|       +-- include
|       +-- lib
|       +-- build_info.md
|       +-- LICENSE
+-- MSVC142_32 ...
+-- MSVC141_64 ...
+-- MSVC141_32 ...
+-- MSVC140_64 ...
+-- MSVC140_32 ...
```
