# Prebuilt binaries OpenCV C++ for Windows
##### Current stable build of gRPC v4.5.5
##### OpenCV [v4.5.5](https://github.com/grpc/grpc/releases/tag/v4.5.5) 

> They can be downloaded separately as zip archives from the  [releases](https://github.com/thommyho/Cpp-OpenCV-Windows-PreBuilts/releases) page


##### Releases

| Version | Commit | Debug | Release  | RelWithDebInfo | MSVC142 32Bit | MSVC142 64Bit | MSVC141 32 Bit | MSVC141 64 Bit | MSVC140 32 Bit | MSVC140 64 Bit | Example |
|---------|------------|-------|----------|----------------|---------------|---------------|----------------|----------------|----------------|----------------|---------|
| [4.5.5](https://github.com/thommyho/Cpp-OpenCV-Windows-PreBuilts/releases/tag/v4.5.5) | 4223495e6cd67011f86b8ecd9be1fa105018f3b1 | :ballot_box_with_check: | :ballot_box_with_check: | :ballot_box_with_check:              | :ballot_box_with_check:             | :ballot_box_with_check:             | :ballot_box_with_check:              | :ballot_box_with_check:              | :ballot_box_with_check:              | :ballot_box_with_check:              | :ballot_box_with_check:       |

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
General configuration for OpenCV 4.5.5 =====================================

  Version control:               4.5.5-dirty

  Platform:
    Timestamp:                   2021-12-26T16:47:37Z
    Host:                        Windows 10.0.19042 AMD64
    CMake:                       3.21.2
    CMake generator:             Visual Studio 16 2019
    CMake build tool:            C:/Program Files (x86)/Microsoft Visual Studio/2019/BuildTools/MSBuild/Current/Bin/MSBuild.exe
    MSVC:                        1929
    Configuration:               Debug Release MinSizeRel RelWithDebInfo

  CPU/HW features:
    Baseline:                    SSE SSE2 SSE3
      requested:                 SSE3
    Dispatched code generation:  SSE4_1 SSE4_2 FP16 AVX AVX2 AVX512_SKX
      requested:                 SSE4_1 SSE4_2 AVX FP16 AVX2 AVX512_SKX
      SSE4_1 (16 files):         + SSSE3 SSE4_1
      SSE4_2 (1 files):          + SSSE3 SSE4_1 POPCNT SSE4_2
      FP16 (0 files):            + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 AVX
      AVX (4 files):             + SSSE3 SSE4_1 POPCNT SSE4_2 AVX
      AVX2 (31 files):           + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 FMA3 AVX AVX2
      AVX512_SKX (5 files):      + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 FMA3 AVX AVX2 AVX_512F AVX512_COMMON AVX512_SKX

  C/C++:
    Built as dynamic libs?:      NO
    C++ standard:                11
    C++ Compiler:                C:/Program Files (x86)/Microsoft Visual Studio/2019/BuildTools/VC/Tools/MSVC/14.29.30133/bin/Hostx64/x64/cl.exe  (ver 19.29.30133.0)
    C++ flags (Release):         /DWIN32 /D_WINDOWS /W4 /GR  /D _CRT_SECURE_NO_DEPRECATE /D _CRT_NONSTDC_NO_DEPRECATE /D _SCL_SECURE_NO_WARNINGS /Gy /bigobj /Oi  /fp:precise     /EHa /wd4127 /wd4251 /wd4324 /wd4275 /wd4512 /wd4589 /MP  /MD /O2 /Ob2 /DNDEBUG 
    C++ flags (Debug):           /DWIN32 /D_WINDOWS /W4 /GR  /D _CRT_SECURE_NO_DEPRECATE /D _CRT_NONSTDC_NO_DEPRECATE /D _SCL_SECURE_NO_WARNINGS /Gy /bigobj /Oi  /fp:precise     /EHa /wd4127 /wd4251 /wd4324 /wd4275 /wd4512 /wd4589 /MP  /MDd /Zi /Ob0 /Od /RTC1 
    C Compiler:                  C:/Program Files (x86)/Microsoft Visual Studio/2019/BuildTools/VC/Tools/MSVC/14.29.30133/bin/Hostx64/x64/cl.exe
    C flags (Release):           /DWIN32 /D_WINDOWS /W3  /D _CRT_SECURE_NO_DEPRECATE /D _CRT_NONSTDC_NO_DEPRECATE /D _SCL_SECURE_NO_WARNINGS /Gy /bigobj /Oi  /fp:precise     /MP   /MD /O2 /Ob2 /DNDEBUG 
    C flags (Debug):             /DWIN32 /D_WINDOWS /W3  /D _CRT_SECURE_NO_DEPRECATE /D _CRT_NONSTDC_NO_DEPRECATE /D _SCL_SECURE_NO_WARNINGS /Gy /bigobj /Oi  /fp:precise     /MP /MDd /Zi /Ob0 /Od /RTC1 
    Linker flags (Release):      /machine:x64  /INCREMENTAL:NO 
    Linker flags (Debug):        /machine:x64  /debug /INCREMENTAL 
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
    JPEG:                        build-libjpeg-turbo (ver 2.1.2-62)
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
           at:                   D:/Jenkins/2/3/4/workspace/OpenCV-Build-Pkg/opencv/build_4.5.5_MSVC142_64/3rdparty/ippicv/ippicv_win/icv
    Intel IPP IW:                sources (2020.0.0)
              at:                D:/Jenkins/2/3/4/workspace/OpenCV-Build-Pkg/opencv/build_4.5.5_MSVC142_64/3rdparty/ippicv/ippicv_win/iw
    Lapack:                      NO
    Eigen:                       NO
    Custom HAL:                  NO
    Protobuf:                    build (3.19.1)

  OpenCL:                        YES (NVD3D11)
    Include path:                D:/Jenkins/2/3/4/workspace/OpenCV-Build-Pkg/opencv/3rdparty/include/opencl/1.2
    Link libraries:              Dynamic load

  Python (for build):            NO

  Install to:                    D:/out/opencv_4.5.5/MSVC142_64/RelWithDebInfo
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
|   ....
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
|   ....
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
|   ....
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
