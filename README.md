# G-CoreStreamsDemo
# Introduction
Set up live streaming in 15 minutes in your iOS project instead of 7 days of work and setting wild parameters of codecs, network, etc. This demo project is a quick tutorial how to stream live video from your own mobile app to an audience of 1 000 000+ viewers like Instagram, Youtube, etc.
# Features
1. HLS & MPEG-DASH playback
2. Video:
    * RTMP streaming
    * Network adaptive bitrate mechanism
    * Source: front and back cameras
    * Orientation: portrait
    * Codec: AVC/H.264
    * Configurable bitrate, resolution, iFrameInterval, encoder profile
3. Audio:
    * Codec: AAC
    * Mute mode
    * Configurable bitrate, sample rate, stereo/mono
    * Processing: noise suppressor, echo cancellation
# Checking with G-Core-Labs demo account
1. Install the app via .apk which is on the path app/build/outputs/apk/debug. Or you can clone this project and run it in Android Studio, where you can test it either by connecting a real device or through an Android emulator
2. Log in using the email and password from the G-Core-Labs demo account
3. On the Streams screen, you can watch the available streams
4. On the Select stream screen, you can select/create a stream to start streaming
5. On the Start Broadcast screen, you can start broadcasting, set the video quality, and select push url or backup push url for streaming
# Quick Start
### 1. Compile
You will need a third party library to implement RTMP streaming. You will need a third party library to implement RTMP streaming. In this project, [rtmp-rtsp-stream-client-java](https://github.com/pedroSG94/rtmp-rtsp-stream-client-java) was used. To use it, you need to specify this in your build.gradle:
``` gradle
allprojects {
  repositories {
    maven { url 'https://jitpack.io' }
  }
}
dependencies {
  implementation 'com.github.pedroSG94.rtmp-rtsp-stream-client-java:rtplibrary:2.1.7'
}
```
# Requirements
* The presence of an Internet connection on the device
* The presence of a camera and microphone on the device.
* Anroid min API 23 
# License
