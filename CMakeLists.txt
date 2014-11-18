cmake_minimum_required(VERSION 2.8.9)

project(MyFirstSlicerExtension)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://github.com/sampada02/MyFirstSlicerExtension")
set(EXTENSION_CATEGORY "Learning")
set(EXTENSION_CONTRIBUTORS "Sampada Bhave (UIOWA)")
set(EXTENSION_DESCRIPTION "This extension is developd as a part of tutorial")
set(EXTENSION_ICONURL "https://raw.github.com/sampada02/MyFirstSlicerExtension/master/MyFirstSlicerExtension.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/MyFirstSlicerExtension/Screenshots/1.png")

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(LineIntensityProfile)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_CPACK})
