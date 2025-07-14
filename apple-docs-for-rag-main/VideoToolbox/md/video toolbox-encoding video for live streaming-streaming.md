

- Video Toolbox
-  Encoding video for live streaming 

Sample Code

# Encoding video for live streaming

Configure a compression session to encode video for live streaming.

Download

macOS 13.3+Xcode 14.3+

## Overview

This sample code project demonstrates how to configure and use a `VTCompressionSession` object to encode video for live streaming.

### Create a compression session

Create a `VTCompressionSession` object and specify the required dimensions and `codecType`. Optionally, specify `sourceImageBufferAttributes` to provide a description of the source pixel buffers.

```
```

### Configure the compression session

Specify the codec profile and level, the expected video source frame rate, and the maximum interval between key frames. Specify the target average bit rate and the data rate limits or the target constant bit rate. Enable temporal compression and frame reordering. Set `kVTCompressionPropertyKey_RealTime` to `kCFBooleanTrue` to indicate this is a live encoding session.

```
```

### Encode video frames

Call `VTCompressionSessionEncodeFrame(_:imageBuffer:presentationTimeStamp:duration:frameProperties:infoFlagsOut:outputHandler:)` and submit each uncompressed frame to the `VTCompressionSession` object for encoding. The object calls the `outputHandler` block for each encoded frame. Check whether a frame drop or error occurs after frame encoding.

Call `VTCompressionSessionCompleteFrames(_:untilPresentationTimeStamp:)` to indicate to the `VTCompressionSession` object that the app submitted all uncompressed video frames for encoding.

### Perform compression and encoding

You can use the movie file `/Assets/video3.m4v` to test this app. Copy the file to your desktop or other working directory, and then open Terminal to that directory and run the following command, where `xxx` is a unique string that Xcode generates. Use autocomplete before the `xxx` component to complete the path for that directory.

`~/Library/Developer/Xcode/DerivedData/VTEncoderForStreaming-xxx/Build/Products/Debug/VTEncoderForStreaming-Swift video3.m4v`

Pass the `--help` option for additional configuration options.

## See Also

### Compression

Encoding video for low-latency conferencing

Configure a compression session to optimize encoding for video-conferencing apps.

Encoding video for offline transcoding

Configure a compression session to transcode video in offline workflows.

VTCompressionSession

An object that compresses video data.

VTDecompressionSession

An object that decompresses video data.

VTFrameSilo

An object that stores sample buffers from a multipass encoding session.

VTMultiPassStorage

An object that stores video encoding metadata from a multipass encoding session.

