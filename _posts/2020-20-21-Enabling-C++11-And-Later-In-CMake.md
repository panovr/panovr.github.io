---
layout: post
title: Enabling C++11 And Later In CMake
date:   2020-02-21 16:50:00
categories: Modern CMake
---

## Setting the C++ standard directly

The simplest way to use a particular C++ standard in your project is to add the following two variable definitions before you define any targets:

```
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)
```

See [CXX_STANDARD](https://cmake.org/cmake/help/latest/prop_tgt/CXX_STANDARD.html) help.