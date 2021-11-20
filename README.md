# zlib-android-build

## Cross-compiles zlib library for Android

This script cross-compiles zlib library for Android (armeabi-v7a, arm64-v8a) using Android NDK and autoconf, as shown in [Use the NDK with other build systems](https://developer.android.com/ndk/guides/other_build_systems#autoconf).

> This script has been tested on Debian GNU/Linux 10 (buster) x86_64 with Android NDK r22b (22.1.7171670).

> This script download zlib source code from zlib official website (https://www.zlib.net/)

> If the script is invoked with no arguments, by default zlib-1.2.11 static libraries are compiled for android-21 arm64-v8a using the Android NDK path provided by ANDROID_NDK environment variable.

### Dependencies:

- Android NDK r22+
- curl
- make

### Android Arch Supported:

- arm (armeabi-v7a)
- arm64 (arm64-v8a)

### TODO:

- Improve message logging, log all events (err, std) in `build.log` file.
- Implement clean callback on error.