# Vita3K iOS build report
- run: https://github.com/SSRplus/test/actions/runs/39893916734
- result: **cancelled**
- date: 2026-10-23 03:18 UTC

## Error lines
```
logs/06-build.log:82:-- Looking for fwrite_unlocked - not found
logs/06-build.log:107:-- Looking for __GLIBC__ - not found
logs/06-build.log:131:-- Looking for malloc.h - not found
logs/06-build.log:217:-- Looking for fopen64 - not found
logs/06-build.log:221:-- Looking for fseeko64 - not found
logs/06-build.log:225:-- Looking for _i64toa - not found
logs/06-build.log:229:-- Looking for itoa - not found
logs/06-build.log:243:-- Looking for _ltoa - not found
logs/06-build.log:281:-- Looking for sqr - not found
logs/06-build.log:369:-- Looking for fdatasync - not found
logs/06-build.log:377:-- Looking for sigtimedwait - not found
logs/06-build.log:393:-- Looking for getauxval - not found
logs/06-build.log:395:-- Looking for elf_aux_info - not found
logs/06-build.log:399:-- Looking for memfd_create - not found
logs/06-build.log:401:-- Looking for posix_fallocate - not found
logs/06-build.log:428:-- Looking for pthread_np.h - not found
```

## 01-get-source.log (last 60 lines)
```
--- files in repo root:
total 15544
drwxr-xr-x   9 runner  staff      288 Oct 23 03:14 .
drwxr-xr-x   3 runner  staff       96 Oct 23 03:14 ..
drwxr-xr-x  14 runner  staff      448 Oct 23 03:14 .git
drwxr-xr-x   3 runner  staff       96 Oct 23 03:14 .github
drwxr-xr-x   2 runner  staff       64 Oct 23 03:14 logs
-rw-r--r--   1 runner  staff        6 Oct 23 03:14 README.md
-rw-r--r--   1 runner  staff    81782 Oct 23 03:14 Vita3K-iOS-port.zip
-rw-r--r--   1 runner  staff  7870306 Oct 23 03:14 Vita3K-Plus-master.zip
drwxr-xr-x   4 runner  staff      128 Oct 23 03:14 work
source zip: Vita3K-Plus-master.zip
src=work/src_unz/Vita3K-Plus-master port=work/port_unz/Vita3K-iOS-port pin=nckstwrt/Vita3K-Plus
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
✔︎ Bottle nasm (3.02)
✔︎ Bottle libplist (2.7.0)
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

## 04-deps.log (last 60 lines)
```
+ '[' -z '' ']'
+ '[' -n /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master ']'
+ '[' -d /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/external/ffmpeg ']'
++ grep -oE '[67]\.[0-9](\.[0-9]+)?'
++ grep -rhoiE 'ffmpeg[-_ /]*(n|version[ =:]*)?[67]\.[0-9](\.[0-9]+)?' /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/external/ffmpeg
++ sort -V
++ tail -1
+ FF_VER=
+ case "$FF_VER" in
+ FF_VER=6.1.1
+ case "$FF_VER" in
+ echo 'FFmpeg version: 6.1.1'
FFmpeg version: 6.1.1
+ '[' '!' -f /Users/runner/work/test/test/ios-deps/lib/libavcodec.a ']'
+ head -60
+ ls /Users/runner/work/test/test/ios-deps /Users/runner/work/test/test/ios-deps/lib
/Users/runner/work/test/test/ios-deps:
bin
Frameworks
include
lib
share

/Users/runner/work/test/test/ios-deps/lib:
cmake
libavcodec.a
libavfilter.a
libavformat.a
libavutil.a
libboost_atomic.a
libboost_filesystem.a
libboost_system.a
libcrypto.a
libcurl.a
libssl.a
libswresample.a
libswscale.a
pkgconfig
+ missing=0
+ for l in libcrypto.a libssl.a libboost_filesystem.a libcurl.a libavcodec.a libavformat.a libavutil.a libswresample.a libswscale.a
+ '[' -f /Users/runner/work/test/test/ios-deps/lib/libcrypto.a ']'
+ for l in libcrypto.a libssl.a libboost_filesystem.a libcurl.a libavcodec.a libavformat.a libavutil.a libswresample.a libswscale.a
+ '[' -f /Users/runner/work/test/test/ios-deps/lib/libssl.a ']'
+ for l in libcrypto.a libssl.a libboost_filesystem.a libcurl.a libavcodec.a libavformat.a libavutil.a libswresample.a libswscale.a
+ '[' -f /Users/runner/work/test/test/ios-deps/lib/libboost_filesystem.a ']'
+ for l in libcrypto.a libssl.a libboost_filesystem.a libcurl.a libavcodec.a libavformat.a libavutil.a libswresample.a libswscale.a
+ '[' -f /Users/runner/work/test/test/ios-deps/lib/libcurl.a ']'
+ for l in libcrypto.a libssl.a libboost_filesystem.a libcurl.a libavcodec.a libavformat.a libavutil.a libswresample.a libswscale.a
+ '[' -f /Users/runner/work/test/test/ios-deps/lib/libavcodec.a ']'
+ for l in libcrypto.a libssl.a libboost_filesystem.a libcurl.a libavcodec.a libavformat.a libavutil.a libswresample.a libswscale.a
+ '[' -f /Users/runner/work/test/test/ios-deps/lib/libavformat.a ']'
+ for l in libcrypto.a libssl.a libboost_filesystem.a libcurl.a libavcodec.a libavformat.a libavutil.a libswresample.a libswscale.a
+ '[' -f /Users/runner/work/test/test/ios-deps/lib/libavutil.a ']'
+ for l in libcrypto.a libssl.a libboost_filesystem.a libcurl.a libavcodec.a libavformat.a libavutil.a libswresample.a libswscale.a
+ '[' -f /Users/runner/work/test/test/ios-deps/lib/libswresample.a ']'
+ for l in libcrypto.a libssl.a libboost_filesystem.a libcurl.a libavcodec.a libavformat.a libavutil.a libswresample.a libswscale.a
+ '[' -f /Users/runner/work/test/test/ios-deps/lib/libswscale.a ']'
+ '[' -d /Users/runner/work/test/test/ios-deps/Frameworks/MoltenVK.framework ']'
+ '[' -f /Users/runner/work/test/test/ios-deps/include/libavcodec/codec_internal.h ']'
+ exit 0
```

## 05-patch.log (last 60 lines)
```
dynarmic MAP_JIT patched: external/dynarmic/externals/oaknut/include/oaknut/code_block.hpp
dynarmic MAP_JIT patched: external/dynarmic/externals/xbyak/xbyak/xbyak.h
dynarmic MAP_JIT patched: external/dynarmic/src/dynarmic/backend/x64/block_of_code.cpp
capstone arch override removed
GLES paths enabled for iOS: vita3k/renderer/src/gl/ring_buffer.cpp
GLES paths enabled for iOS: vita3k/renderer/src/gl/screen_render.cpp
GLES paths enabled for iOS: vita3k/renderer/src/gl/texture.cpp
GLES paths enabled for iOS: vita3k/renderer/src/gl/sync_state.cpp
GLES paths enabled for iOS: vita3k/renderer/src/gl/renderer.cpp
all iOS patches applied
```

## 06-build.log (last 60 lines)
```
[487/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/GenericCodeGen/Link.cpp.o
[488/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/CInterface/glslang_c_interface.cpp.o
[489/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/OSDependent/Unix/ossource.cpp.o
[490/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/attribute.cpp.o
[491/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/Constant.cpp.o
[492/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/glslang_tab.cpp.o
[493/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/InfoSink.cpp.o
[494/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/IntermTraverse.cpp.o
[495/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/iomapper.cpp.o
[496/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/Initialize.cpp.o
[497/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/Intermediate.cpp.o
[498/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/ParseContextBase.cpp.o
[499/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/PoolAlloc.cpp.o
[500/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/RemoveTree.cpp.o
[501/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/Scan.cpp.o
[502/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/ParseHelper.cpp.o
[503/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/SpirvIntrinsics.cpp.o
[504/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/ShaderLang.cpp.o
[505/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/Versions.cpp.o
[506/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/intermOut.cpp.o
[507/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/SymbolTable.cpp.o
[508/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/limits.cpp.o
[509/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/parseConst.cpp.o
[510/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/linkValidate.cpp.o
[511/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/reflection.cpp.o
[512/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/preprocessor/Pp.cpp.o
[513/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/preprocessor/PpAtom.cpp.o
[514/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/preprocessor/PpContext.cpp.o
[515/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/preprocessor/PpScanner.cpp.o
[516/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/preprocessor/PpTokens.cpp.o
[517/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/MachineIndependent/propagateNoContraction.cpp.o
[518/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/__/SPIRV/InReadableOrder.cpp.o
[519/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/__/SPIRV/Logger.cpp.o
[520/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/__/SPIRV/SpvPostProcess.cpp.o
[521/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/__/SPIRV/GlslangToSpv.cpp.o
[522/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/__/SPIRV/SpvBuilder.cpp.o
[523/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/__/SPIRV/doc.cpp.o
[524/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/__/SPIRV/SpvTools.cpp.o
[525/1000] Linking CXX static library external/SPIRV-Cross/libspirv-cross-core.a
[526/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/__/SPIRV/CInterface/spirv_c_interface.cpp.o
[527/1000] Linking CXX static library external/pugixml/libpugixml.a
[528/1000] Building CXX object external/glslang/glslang/CMakeFiles/glslang.dir/__/SPIRV/disassemble.cpp.o
[529/1000] Building C object external/psvpfstools/libb64/CMakeFiles/libb64.dir/src/cencode.c.o
[530/1000] Building C object external/psvpfstools/libb64/CMakeFiles/libb64.dir/src/cdecode.c.o
[531/1000] Building C object external/psvpfstools/libzrif/CMakeFiles/libzRIF.dir/src/keyflate.c.o
[532/1000] Linking CXX static library vita3k/input/libinput.a
[533/1000] Building CXX object external/psvpfstools/libzrif/CMakeFiles/libzRIF.dir/src/licdec.cpp.o
[534/1000] Building CXX object vita3k/config/CMakeFiles/config.dir/src/settings.cpp.o
[535/1000] Building CXX object vita3k/config/CMakeFiles/config.dir/version.cpp.o
[536/1000] Linking CXX static library vita3k/cpu/libcpu.a
[537/1000] Building CXX object vita3k/codec/CMakeFiles/codec.dir/src/atrac9.cpp.o
[538/1000] Building CXX object vita3k/codec/CMakeFiles/codec.dir/src/decoder.cpp.o
[539/1000] Building CXX object external/SPIRV-Cross/CMakeFiles/spirv-cross-glsl.dir/spirv_glsl.cpp.o
[540/1000] Building CXX object vita3k/codec/CMakeFiles/codec.dir/src/aac.cpp.o
[541/1000] Building CXX object vita3k/codec/CMakeFiles/codec.dir/src/h264.cpp.o
[542/1000] Building CXX object vita3k/codec/CMakeFiles/codec.dir/src/mjpeg.cpp.o
[543/1000] Building CXX object vita3k/codec/CMakeFiles/codec.dir/src/mp3.cpp.o
[544/1000] Building CXX object vita3k/codec/CMakeFiles/codec.dir/src/pcm.cpp.o
[545/1000] Building CXX object vita3k/config/CMakeFiles/config.dir/src/config.cpp.o
[546/1000] Building CXX object vita3k/gxm/CMakeFiles/gxm.dir/src/color.cpp.o
```
