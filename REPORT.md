# Vita3K iOS build report
- run: https://github.com/SSRplus/test/actions/runs/39025591285
- result: **success**
- date: 2026-10-17 10:43 UTC

## Error lines
```
logs/06-build.log:52:-- Looking for fwrite_unlocked - not found
logs/06-build.log:77:-- Looking for __GLIBC__ - not found
logs/06-build.log:101:-- Looking for malloc.h - not found
logs/06-build.log:187:-- Looking for fopen64 - not found
logs/06-build.log:191:-- Looking for fseeko64 - not found
logs/06-build.log:195:-- Looking for _i64toa - not found
logs/06-build.log:199:-- Looking for itoa - not found
logs/06-build.log:213:-- Looking for _ltoa - not found
logs/06-build.log:251:-- Looking for sqr - not found
logs/06-build.log:339:-- Looking for fdatasync - not found
logs/06-build.log:347:-- Looking for sigtimedwait - not found
logs/06-build.log:363:-- Looking for getauxval - not found
logs/06-build.log:365:-- Looking for elf_aux_info - not found
logs/06-build.log:369:-- Looking for memfd_create - not found
logs/06-build.log:371:-- Looking for posix_fallocate - not found
logs/06-build.log:398:-- Looking for pthread_np.h - not found
logs/06-build.log:2204:ld: warning: ignoring duplicate libraries: '-lbz2', '-lc++', '-liconv', '-lz', 'external/libminiz.a', 'external/psvpfstools/psvpfsparser/cmake/libpsvpfsparser.a', 'vita3k/app/libapp.a', 'vita3k/audio/libaudio.a', 'vita3k/compat/libcompat.a', 'vita3k/config/libconfig.a', 'vita3k/ctrl/libctrl.a', 'vita3k/display/libdisplay.a', 'vita3k/emuenv/libemuenv.a', 'vita3k/gdbstub/libgdbstub.a', 'vita3k/gxm/libgxm.a', 'vita3k/http/libhttp.a', 'vita3k/ime/libime.a', 'vita3k/io/libio.a', 'vita3k/lang/liblang.a', 'vita3k/mem/libmem.a', 'vita3k/module/libmodule.a', 'vita3k/modules/libmodules.a', 'vita3k/motion/libmotion.a', 'vita3k/net/libnet.a', 'vita3k/overlay/liboverlay.a', 'vita3k/packages/libpackages.a', 'vita3k/patch/libpatch.a', 'vita3k/renderer/librenderer.a', 'vita3k/shader/libshader.a', 'vita3k/touch/libtouch.a', 'vita3k/util/libutil.a'
logs/06-build.log:2205:ld: warning: reducing alignment of section __DATA,__common from 0x8000 to 0x4000 because it exceeds segment maximum alignment
```

## 01-get-source.log (last 60 lines)
```
--- files in repo root:
total 15544
drwxr-xr-x   9 runner  staff      288 Oct 17 10:37 .
drwxr-xr-x   3 runner  staff       96 Oct 17 10:37 ..
drwxr-xr-x  14 runner  staff      448 Oct 17 10:37 .git
drwxr-xr-x   3 runner  staff       96 Oct 17 10:37 .github
drwxr-xr-x   3 runner  staff       96 Oct 17 10:37 logs
-rw-r--r--   1 runner  staff        6 Oct 17 10:37 README.md
-rw-r--r--   1 runner  staff    81482 Oct 17 10:37 Vita3K-iOS-port.zip
-rw-r--r--   1 runner  staff  7870306 Oct 17 10:37 Vita3K-Plus-master.zip
drwxr-xr-x   4 runner  staff      128 Oct 17 10:37 work
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

## 04-deps.log (last 60 lines)
```
+ '[' -z '' ']'
+ '[' -n /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master ']'
+ '[' -d /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/external/ffmpeg ']'
++ grep -rhoiE 'ffmpeg[-_ /]*(n|version[ =:]*)?[67]\.[0-9](\.[0-9]+)?' /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/external/ffmpeg
++ grep -oE '[67]\.[0-9](\.[0-9]+)?'
++ sort -V
++ tail -1
+ FF_VER=
+ case "$FF_VER" in
+ FF_VER=6.1.1
+ case "$FF_VER" in
+ echo 'FFmpeg version: 6.1.1'
FFmpeg version: 6.1.1
+ '[' '!' -f /Users/runner/work/test/test/ios-deps/lib/libavcodec.a ']'
+ ls /Users/runner/work/test/test/ios-deps /Users/runner/work/test/test/ios-deps/lib
+ head -60
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
  149 | #define HTONLL(x)       (x) = htonll((__uint64_t)x)
      |         ^
In file included from /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/app/src/app_init.cpp:41:
In file included from /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/net/include/net/state.h:20:
In file included from /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/net/include/net/epoll.h:3:
In file included from /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/net/include/net/socket.h:20:
/Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/net/include/net/types.h:30:9: warning: 'NTOHLL' macro redefined [-Wmacro-redefined]
   30 | #define NTOHLL(x) ((((uint64_t)ntohl((x) & 0xFFFFFFFFUL)) << 32) | ntohl((uint32_t)((x) >> 32)))
      |         ^
/Applications/Xcode_16.4.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/SDKs/iPhoneOS18.5.sdk/usr/include/sys/_endian.h:146:9: note: previous definition is here
  146 | #define NTOHLL(x)       (x) = ntohll((__uint64_t)x)
      |         ^
/Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/app/src/app_init.cpp:200:17: warning: enumeration value 'CustomDriver' not handled in switch [-Wswitch]
  200 |         switch (setting) {
      |                 ^~~~~~~
/Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/app/src/app_init.cpp:200:17: note: add missing switch cases
  200 |         switch (setting) {
      |                 ^
  201 |         case config::RestartRequiredSetting::CpuOpt:
  202 |             runtime_current.cpu_opt = previous_current.cpu_opt;
  203 |             break;
  204 |         case config::RestartRequiredSetting::BackendRenderer:
  205 |             runtime_current.backend_renderer = previous_current.backend_renderer;
  206 |             break;
  207 |         case config::RestartRequiredSetting::GraphicsDevice:
  208 |             runtime_current.gpu_idx = previous_current.gpu_idx;
  209 |             break;
  210 | #ifdef __ANDROID__
  211 |         case config::RestartRequiredSetting::CustomDriver:
  212 |             runtime_current.custom_driver_name = previous_current.custom_driver_name;
  213 |             break;
  214 | #endif
  215 |         case config::RestartRequiredSetting::HighAccuracy:
3 warnings generated.
[991/1001] Linking CXX static library vita3k/ctrl/libctrl.a
[992/1001] Linking CXX static library external/libcppcommon.a
[993/1001] Building CXX object vita3k/app/CMakeFiles/app.dir/src/session_controller.cpp.o
[994/1001] Building CXX object vita3k/CMakeFiles/vita3k.dir/__/ios/ios_jit.cpp.o
[995/1001] Building CXX object vita3k/app/CMakeFiles/app.dir/src/user.cpp.o
[996/1001] Building CXX object vita3k/CMakeFiles/vita3k.dir/performance.cpp.o
[997/1001] Linking CXX static library vita3k/app/libapp.a
[998/1001] Building CXX object vita3k/CMakeFiles/vita3k.dir/interface.cpp.o
[999/1001] Building OBJCXX object vita3k/CMakeFiles/vita3k.dir/__/ios/ios_main.mm.o
In file included from /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/ios/ios_main.mm:51:
In file included from /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/app/include/app/session_controller.h:21:
In file included from /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/renderer/include/renderer/state.h:23:
In file included from /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/renderer/include/renderer/types.h:23:
In file included from /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/shader/include/shader/spirv_recompiler.h:21:
In file included from /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/shader/include/shader/usse_translator_types.h:20:
In file included from /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/shader/include/shader/usse_types.h:20:
/Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/util/include/util/log.h:20:9: warning: 'SPDLOG_ACTIVE_LEVEL' macro redefined [-Wmacro-redefined]
   20 | #define SPDLOG_ACTIVE_LEVEL SPDLOG_LEVEL_TRACE
      |         ^
/Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/external/spdlog/include/spdlog/common.h:240:13: note: previous definition is here
  240 |     #define SPDLOG_ACTIVE_LEVEL SPDLOG_LEVEL_INFO
      |             ^
1 warning generated.
[1000/1001] Linking CXX executable bin/Vita3K.app/Vita3K
ld: warning: ignoring duplicate libraries: '-lbz2', '-lc++', '-liconv', '-lz', 'external/libminiz.a', 'external/psvpfstools/psvpfsparser/cmake/libpsvpfsparser.a', 'vita3k/app/libapp.a', 'vita3k/audio/libaudio.a', 'vita3k/compat/libcompat.a', 'vita3k/config/libconfig.a', 'vita3k/ctrl/libctrl.a', 'vit
ld: warning: reducing alignment of section __DATA,__common from 0x8000 to 0x4000 because it exceeds segment maximum alignment
```

## 07-package.log (last 60 lines)
```
+ SRC=/Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master
+ PORT=/Users/runner/work/test/test/work/port_unz/Vita3K-iOS-port
+ OUT=/Users/runner/work/test/test/out
+ export IOS_DEPS=/Users/runner/work/test/test/ios-deps
+ IOS_DEPS=/Users/runner/work/test/test/ios-deps
+ rm -rf Payload /Users/runner/work/test/test/out
+ mkdir -p /Users/runner/work/test/test/out
++ find /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/build-ios -maxdepth 4 -type d -name Vita3K.app
++ head -1
+ APP=/Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/build-ios/bin/Vita3K.app
+ '[' -z /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/build-ios/bin/Vita3K.app ']'
+ mkdir -p Payload
+ cp -R /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/build-ios/bin/Vita3K.app Payload/Vita3K.app
+ cp /Users/runner/work/test/test/work/port_unz/Vita3K-iOS-port/ios/Info.plist Payload/Vita3K.app/Info.plist
+ '[' -d Payload/Vita3K.app/data ']'
+ '[' -d Payload/Vita3K.app/shaders-builtin ']'
+ '[' -f /Users/runner/work/test/test/work/port_unz/Vita3K-iOS-port/ios/AppIcon.png ']'
+ true
+ '[' -f /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/Vita3K.png ']'
+ cp /Users/runner/work/test/test/work/src_unz/Vita3K-Plus-master/vita3k/Vita3K.png Payload/Vita3K.app/Icon.png
+ mkdir -p Payload/Vita3K.app/Frameworks
+ cp -R /Users/runner/work/test/test/ios-deps/Frameworks/MoltenVK.framework Payload/Vita3K.app/Frameworks/
+ ldid -S Payload/Vita3K.app/Frameworks/MoltenVK.framework/MoltenVK
+ ldid -S/Users/runner/work/test/test/work/port_unz/Vita3K-iOS-port/ios/entitlements.plist Payload/Vita3K.app/Vita3K
+ zip -qry /Users/runner/work/test/test/out/Vita3K.ipa Payload
+ cp /Users/runner/work/test/test/out/Vita3K.ipa /Users/runner/work/test/test/out/Vita3K.tipa
+ ls -la /Users/runner/work/test/test/out
total 63912
drwxr-xr-x   4 runner  staff       128 Oct 17 10:43 .
drwxr-xr-x  13 runner  staff       416 Oct 17 10:42 ..
-rw-r--r--   1 runner  staff  15890688 Oct 17 10:43 Vita3K.ipa
-rw-r--r--   1 runner  staff  15890688 Oct 17 10:43 Vita3K.tipa
```
