Using ifm3d in a CMake Project
=================================

To use ifm3d in your project `myproj`, use:

```cmake
cmake_minimum_required (VERSION 3.0)
project (myproj)

find_package (ifm3d REQUIRED COMPONENTS camera framgegrabber image pcicclient)

add_executable (myapp main.cpp)
target_link_libraries (myapp ifm3d::ifm3d_camera_shared ifm3d::ifm3d_framegrabber_shared ifm3d::ifm3d_image_shared ifm3d::ifm3d_pcicclient_shared)
```

Compile definitions and options will be added automatically to your target as
needed.
