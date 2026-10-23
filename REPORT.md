# Vita3K iOS build report
- run: https://github.com/SSRplus/test/actions/runs/39903308466
- result: **failure**
- date: 2026-10-23 05:01 UTC

## Error lines
```
logs/03c-metal-test.log:27:FAILED: [code=1] CMakeFiles/metal_shader_test.dir/Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/shader/src/spirv_to_msl.cpp.o 
logs/03c-metal-test.log:29:/Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/shader/src/spirv_to_msl.cpp:56:21: error: no member named 'ios_use_framebuffer_fetch_subpasses' in 'spirv_cross::CompilerMSL::Options'; did you mean 'use_framebuffer_fetch_subpasses'?
logs/03c-metal-test.log:49:TEST-BUILD: compile FAILED
```

## 01-get-source.log (last 60 lines)
```
--- files in repo root:
total 31096
drwxr-xr-x  10 runner  staff      320 Oct 23 05:00 .
drwxr-xr-x   3 runner  staff       96 Oct 23 04:59 ..
drwxr-xr-x  14 runner  staff      448 Oct 23 05:00 .git
drwxr-xr-x   3 runner  staff       96 Oct 23 05:00 .github
drwxr-xr-x   3 runner  staff       96 Oct 23 05:00 logs
-rw-r--r--   1 runner  staff  7965539 Oct 23 05:00 project.zip
-rw-r--r--   1 runner  staff        6 Oct 23 05:00 README.md
-rw-r--r--   1 runner  staff    75769 Oct 23 05:00 Vita3K-iOS-port.zip
-rw-r--r--   1 runner  staff  7870306 Oct 23 05:00 Vita3K-Plus-master.zip
drwxr-xr-x   5 runner  staff      160 Oct 23 05:00 work
unpacking project.zip
work/project
work/project/Vita3K-iOS-port
work/project/Vita3K-iOS-port/build-ios.yml
work/project/Vita3K-iOS-port/metal
work/project/Vita3K-iOS-port/metal/tests
work/project/Vita3K-iOS-port/metal/shader
work/project/Vita3K-iOS-port/ios
work/project/Vita3K-iOS-port/ios/ffmpeg_ios.cmake
work/project/Vita3K-iOS-port/ios/entitlements.plist
work/project/Vita3K-iOS-port/ios/ios_ui.inc.mm
work/project/Vita3K-iOS-port/ios/ios_jit.cpp
work/project/Vita3K-iOS-port/ios/ios_main.mm
work/project/Vita3K-iOS-port/ios/ios_net_helper.cpp
work/project/Vita3K-iOS-port/ios/ios_jit.h
work/project/Vita3K-iOS-port/ios/Info.plist
work/project/Vita3K-iOS-port/ios/ios-toolchain.cmake
work/project/Vita3K-iOS-port/README.md
work/project/Vita3K-iOS-port/scripts
work/project/Vita3K-iOS-port/scripts/deps-ios.sh
work/project/Vita3K-iOS-port/scripts/apply_metal_patches.py
work/project/Vita3K-iOS-port/scripts/make-report.sh
work/project/Vita3K-iOS-port/scripts/apply_ios_patches.py
work/project/Vita3K-iOS-port/scripts/make-ipa.sh
work/project/Vita3K-iOS-port/scripts/build-ios.sh
work/project/Vita3K-iOS-port/scripts/metal-shader-test.sh
work/project/Vita3K-iOS-port/scripts/fetch-submodules.sh
work/project/Vita3K-iOS-port/vita3k-ime
work/project/Vita3K-iOS-port/vita3k-ime/text.h
work/project/Vita3K-iOS-port/vita3k-ime/event.h
work/project/Vita3K-iOS-port/vita3k-ime/SceIme.cpp
source zip: work/project/Vita3K-Plus-master.zip
src=work/src_unz/Vita3K-Plus-master port=work/project/Vita3K-iOS-port pin=nckstwrt/Vita3K-Plus
```

## 02-tools.log (last 60 lines)
```
[33mWarning:[0m cmake 4.4.3 is already installed and up-to-date.
To reinstall 4.4.3, run:
  brew reinstall cmake
[33mWarning:[0m ninja 1.13.2 is already installed and up-to-date.
To reinstall 1.13.2, run:
  brew reinstall ninja
[33mWarning:[0m pkgconf 3.0.7 is already installed and up-to-date.
To reinstall 3.0.7, run:
  brew reinstall pkgconf
[32m==>[0m [1mDownloading bottle manifests[0m
✔︎ Bottle Manifest ldid (2.1.5_1)
✔︎ Bottle Manifest nasm (3.02)
[34m==>[0m [1mWould install 2 formulae:[0m
ldid nasm
[34m==>[0m [1mWould install 1 dependency for ldid:[0m
libplist
[32m==>[0m [1mFetching downloads for: [32mldid[39m and [32mnasm[39m[0m
✔︎ Bottle Manifest libplist (2.7.0)
✔︎ Bottle ldid (2.1.5_1)
✔︎ Bottle libplist (2.7.0)
✔︎ Bottle nasm (3.02)
[32m==>[0m [1mInstalling ldid dependency: [32mlibplist[39m[0m
[34m==>[0m [1mPouring libplist--2.7.0.arm64_sequoia.bottle.tar.gz[0m
🍺  /opt/homebrew/Cellar/libplist/2.7.0: 32 files, 604.1KB
[32m==>[0m [1mInstalling [32mldid[39m[0m
[34m==>[0m [1mPouring ldid--2.1.5_1.arm64_sequoia.bottle.1.tar.gz[0m
🍺  /opt/homebrew/Cellar/ldid/2.1.5_1: 6 files, 270KB
[34m==>[0m [1mPouring nasm--3.02.arm64_sequoia.bottle.tar.gz[0m
🍺  /opt/homebrew/Cellar/nasm/3.02: 12 files, 3MB
Xcode 16.4
Build version 16F6
cmake version 4.4.3

CMake suite maintained and supported by Kitware (kitware.com/cmake).
```

## 03-submodules.log (last 60 lines)
```
pins from nckstwrt/Vita3K-Plus:       28
pins from Vita3K/Vita3K:       28
pinned submodules total:       28
== external/boost  (https://github.com/Vita3K/ext-boost)  pin=ff5f55bd97a93b23d6e5cb6d192290fb49b3f002
== external/capstone  (https://github.com/aquynh/capstone.git)  pin=cd6dd7b75d126a855be1f9f76570ee5a850c6061
== external/dirent  (https://github.com/tronkko/dirent)  pin=39c1f1bc98ef3326237d03006f35d7dd44620e43
== external/dlmalloc  (https://github.com/Vita3K/dlmalloc)  pin=e98f4ee160380d7c39dc1f04e7488bcf0770d391
== external/ffmpeg  (https://github.com/Vita3K/ffmpeg-core.git)  pin=02f4f2691b0efffff8923235baf146a87fc37263
== external/glslang  (https://github.com/KhronosGroup/glslang)  pin=fc9889c889561c5882e83819dcaffef5ed45529b
== external/googletest  (https://github.com/google/googletest)  pin=6910c9d9165801d8827d628cb72eb7ea9dd538c5
== external/libfat16  (https://github.com/Vita3K/libfat16)  pin=d9a890b712dcdb46d3d33230997efc59f5ad8d62
== external/printf  (https://github.com/Vita3K/printf)  pin=c75def6db38f9978c55e8d27227858df911cd727
== external/pugixml  (https://github.com/zeux/pugixml)  pin=ee86beb30e4973f5feffe3ce63bfa4fbadf72f38
== external/sdl  (https://github.com/libsdl-org/SDL.git)  pin=7f3ae3d57459e59943a4ecfefc8f6277ec6bf540
== external/spdlog  (https://github.com/gabime/spdlog)  pin=48bcf39a661a13be22666ac64db8a7f886f2637e
== external/SPIRV-Cross  (https://github.com/KhronosGroup/SPIRV-Cross.git)  pin=d8e3e2b141b8c8a167b2e3984736a6baacff316c
== external/stb  (https://github.com/nothings/stb)  pin=f0569113c93ad095470c54bf34a17b36646bbbb5
== external/vita-toolchain  (https://github.com/vitasdk/vita-toolchain.git)  pin=77f17b979678e7af0acfe708dc97a45ca6fd55e2
== external/VulkanMemoryAllocator-Hpp  (https://github.com/YaaZ/VulkanMemoryAllocator-Hpp)  pin=2059f0fdd73492b03d60a90c73e5038224b99093
== external/yaml-cpp  (https://github.com/jbeder/yaml-cpp)  pin=2f86d13775d119edbb69af52e5f566fd65c6953b
== external/psvpfstools  (https://github.com/Vita3K/psvpfstools.git)  pin=ab1aa9b36388843f6a9f8dc86b1746f1f2a7e557
== external/xxHash  (https://github.com/Cyan4973/xxHash)  pin=e626a72bc2321cd320e953a0ccf1584cad60f363
== external/dynarmic  (https://github.com/Vita3K/dynarmic.git)  pin=86458a0bd369d63ba4c2ef812cacbb6c9080c065
== external/fmt  (https://github.com/fmtlib/fmt.git)  pin=e424e3f2e607da02742f73db84873b8084fc714c
== external/LibAtrac9  (https://github.com/Vita3K/LibAtrac9.git)  pin=82767fe38823c32536726ea798f392b0b49e66b9
== external/tracy  (https://github.com/wolfpld/tracy.git)  pin=05cceee0df3b8d7c6fa87e9638af311dbabc63cb
== external/nativefiledialog-extended  (https://github.com/btzy/nativefiledialog-extended.git)  pin=86d5f2005fe1c00747348a12070fec493ea2407e
== external/cubeb  (https://github.com/mozilla/cubeb.git)  pin=f8633c0c9217ed5499fdda391946d416c52e6809
== external/concurrentqueue  (https://github.com/cameron314/concurrentqueue.git)  pin=6dd38b8a1dbaa7863aa907045f32308a56a6ff5d
== external/libadrenotools  (https://github.com/bylaws/libadrenotools)  pin=8fae8ce254dfc1344527e05301e43f37dea2df80
== external/substitute  (https://github.com/Vita3K/substitute.git)  pin=319da6b563d8da689f3b9df2fbb839edd41a1943
```

## 03b-metal-patch.log (last 60 lines)
```
added vita3k/shader/include/shader/gxp_to_msl.h
added vita3k/shader/include/shader/spirv_to_msl.h
added vita3k/shader/src/spirv_to_msl.cpp
added vita3k/shader/src/gxp_to_msl.cpp
metal phase 1 patches applied
```

## 03c-metal-test.log (last 60 lines)
```
-- The C compiler identification is AppleClang 17.0.0.17000013
-- The CXX compiler identification is AppleClang 17.0.0.17000013
-- The OBJCXX compiler identification is AppleClang 17.0.0.17000013
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Detecting OBJCXX compiler ABI info
-- Detecting OBJCXX compiler ABI info - done
-- Check for working OBJCXX compiler: /usr/bin/c++ - skipped
-- SPIRV-Cross: Finding Git version for SPIRV-Cross.
-- Found Git: /opt/homebrew/bin/git (found version "2.55.0")
-- SPIRV-Cross: Git hash: d8e3e2b
-- Configuring done (3.5s)
-- Generating done (0.0s)
-- Build files have been written to: /Users/runner/work/test/test/metal-test/build
[1/12] Building CXX object spirv-cross/CMakeFiles/spirv-cross-core.dir/spirv_cfg.cpp.o
[2/12] Building CXX object spirv-cross/CMakeFiles/spirv-cross-core.dir/spirv_cross_parsed_ir.cpp.o
[3/12] Building CXX object spirv-cross/CMakeFiles/spirv-cross-core.dir/spirv_parser.cpp.o
[4/12] Building CXX object CMakeFiles/metal_shader_test.dir/Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/shader/src/spirv_to_msl.cpp.o
FAILED: [code=1] CMakeFiles/metal_shader_test.dir/Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/shader/src/spirv_to_msl.cpp.o 
/usr/bin/c++  -I/Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/shader/include -I/Users/runner/work/test/test/work/project/Vita3K-iOS-port/metal/tests/metal_shader_test -I/Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/external/SPIRV-Cross -O3 -DNDEBUG -std=gnu++20 -
/Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/shader/src/spirv_to_msl.cpp:56:21: error: no member named 'ios_use_framebuffer_fetch_subpasses' in 'spirv_cross::CompilerMSL::Options'; did you mean 'use_framebuffer_fetch_subpasses'?
   56 |         msl_options.ios_use_framebuffer_fetch_subpasses = options.framebuffer_fetch && options.ios;
      |                     ^~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
      |                     use_framebuffer_fetch_subpasses
/Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/external/SPIRV-Cross/spirv_msl.hpp:374:8: note: 'use_framebuffer_fetch_subpasses' declared here
  374 |                 bool use_framebuffer_fetch_subpasses = false;
      |                      ^
1 error generated.
[5/12] Building OBJCXX object CMakeFiles/metal_shader_test.dir/test_main.mm.o
/Users/runner/work/test/test/work/project/Vita3K-iOS-port/metal/tests/metal_shader_test/test_main.mm:133:14: warning: 'fastMathEnabled' is deprecated: first deprecated in macOS 15.0 - Use mathMode instead [-Wdeprecated-declarations]
  133 |         opts.fastMathEnabled = NO;
      |              ^
/Applications/Xcode_16.4.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX.sdk/System/Library/Frameworks/Metal.framework/Headers/MTLLibrary.h:282:39: note: 'fastMathEnabled' has been explicitly marked deprecated here
  282 | @property (readwrite, nonatomic) BOOL fastMathEnabled API_DEPRECATED("Use mathMode instead", macos(10.11, 15.0), ios(8.0, 18.0));
      |                                       ^
1 warning generated.
[6/12] Building CXX object spirv-cross/CMakeFiles/spirv-cross-core.dir/spirv_cross.cpp.o
[7/12] Building CXX object spirv-cross/CMakeFiles/spirv-cross-glsl.dir/spirv_glsl.cpp.o
[8/12] Building CXX object spirv-cross/CMakeFiles/spirv-cross-msl.dir/spirv_msl.cpp.o
ninja: build stopped: subcommand failed.
TEST-BUILD: compile FAILED
```
