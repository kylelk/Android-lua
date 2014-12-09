Android-lua
===========

lua command line interpreter for Android.


== Building ==

To build the lua interpreter run the Android NDK build script inside this directory.
this will create the folders libs, and obj. 

the striped execuable will be in `libs/armeabi/lua`

the non striped executable will be in `obj/local/armeabi/lua`

== Installing ==

To install and run the lua interpreter on an Android device a Terminal emulator must be used, Such as [Terminal IDE](https://play.google.com/store/apps/details?id=com.spartacusrex.spartacuside&hl=en).

The command line tool can be run without root permissions by executing the binary in the app's private memory. 

1. Tranfer the lua binary to your Android device.
2. copy lua to the Terminal's `bin` directory, for Terminal IDE it is `~/local/bin/`, the apps home folder is located in **/data/data/ + PACKAGE_NAME**. The apps private memory can only be accessed by the app itself, copy lua using the command `cp /sdcard/lua ~/local/bin/`.  
3. give lua binary executable permission using `chmod +x ~/local/bin/lua`.
4. restart the Terminal emulator app.

Lua is now installed on your android device, lua scripts can be run using `lua FileName.lua`.

