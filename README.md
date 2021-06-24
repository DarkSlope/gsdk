# DarkSlope Notes: Cross-compiling for Linux

It is possible to cross-compile this from Windows for Linux via the UE4 Clang toolchain and CMake with Ninja target.  Make sure Ninja is installed, use the Ninja target in CMake and set the toolchain file to use the PhysX Linux cross compile CMake toolchain file from UE4: Engine/Source/ThirdParty/PhysX3/Externals/CMakeModules/linux/LinuxCrossToolchain.x86_64-unknown-linux-gnu.cmake

Currently you will also have to edit the hardcoded path in CMakeLists.txt for the Clang C++ stdlib headers from UE4 

    target_include_directories(GSDK_CPP PRIVATE <YOUR_UE4_ROOT>/Engine/Source/ThirdParty/Linux/LibCxx/include/c++/v1)


# PlayFab Game Server SDK
[![C++](https://img.shields.io/nuget/v/com.playfab.cppgsdk.v140?style=flat-square&label=C%2B%2B)](https://www.nuget.org/packages/com.playfab.cppgsdk.v140)
[![C#](https://img.shields.io/nuget/v/com.playfab.csharpgsdk?style=flat-square&label=C%23)](https://www.nuget.org/packages/com.playfab.csharpgsdk)
[![Java](https://img.shields.io/maven-central/v/com.playfab/gameserverSDK?style=flat-square&label=Java)](https://mvnrepository.com/artifact/com.playfab/gameserverSDK)

## Overview

PlayFab Game Server SDK for C#, C++, and Java environments.  The GSDK is used to integrate with PlayFab Multiplayer Servers.

## Prerequisites

[getting started guide](https://docs.microsoft.com/en-us/gaming/playfab/features/multiplayer/servers/integrating-game-servers-with-gsdk)

## Samples

Check the [gsdkSamples](https://github.com/PlayFab/gsdkSamples) repo.

## Contact Us

We love to hear from our developer community!
Do you have ideas on how we can make our products and services better?

Our Developer Success Team can assist with answering any questions as well as process any feedback you have about PlayFab services.

[Forums, Support and Knowledge Base](https://community.playfab.com/index.html)

## Contributing

We are more than happy to accept external contributions! If you want to propose a small code change, feel free to open a Pull Request directly. If you plan to do a bigger change, it would be better if you open an issue describing your proposed design in order to get feedback from project maintainers.

## Release Notes

Please navigate into the respective language folders.

## Copyright and Licensing Information

  Apache License --
  Version 2.0, January 2004
  http://www.apache.org/licenses/

  Full details available within the LICENSE file.
