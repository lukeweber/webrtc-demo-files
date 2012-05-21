webrtc-demo-files
=================

webrtc android audio demo (compiling)

* libs contains the libs for android_test located at webrtc/src/voice_engine/main/test/android/android_test
* diff has the changes in webrtc as of this date to be able to compile

Note that I changed the path in jni/Android.mk to be a local path on my machine.
If you want to compile, you'll have to apply the diff to webrtc and then modify
this path, then run ndk-build at webrtc/src/voice_engine/main/test/android/android_test

Also to use the libs only:
* you'll need to change the file,
/home/luke/webrtcproj/trunk/src/voice_engine/main/test/android/android_test/AndroidTest.java, to update the includes
* import  webrtc/src/voice_engine/main/test/android/android_test as an existing
  project in eclipse.
* build in eclipse
