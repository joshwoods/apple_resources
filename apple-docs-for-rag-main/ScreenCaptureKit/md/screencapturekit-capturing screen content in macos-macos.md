

- ScreenCaptureKit
-  Capturing screen content in macOS 

Sample Code

# Capturing screen content in macOS

Stream desktop content like displays, apps, and windows by adopting screen capture in your app.

Download

macOS 15.0+Xcode 16.0+

## Overview

This sample shows how to add high-performance screen capture to your Mac app by using ScreenCaptureKit. The sample explores how to create content filters to capture the displays, apps, and windows you choose. It then shows how to configure your stream output, retrieve video frames and audio samples, and update a running stream.

Note

This sample code project is associated with WWDC24 session 10088: Capture HDR content with ScreenCaptureKit.

### Configure the sample code project

To run this sample app, you’ll need the following:

- A Mac with macOS 15 or later

- Xcode 16 or later

The first time you run this sample, the system prompts you to grant the app Screen Recording permission. After you grant permission, you need to restart the app to enable capture.

### Create a content filter

Displays, running apps, and windows are the shareable content on a device. The sample uses the SCShareableContent class to retrieve the items in the form of SCDisplay, SCRunningApplication, and SCWindow objects respectively.

```
```

Before the sample begins capture, it creates an SCContentFilter object to specify the content to capture. The sample provides two options that allow for capturing either a single window or an entire display. When the capture type is set to capture a window, the app creates a content filter that only includes that window.

```
```

When a user specifies to capture the entire display, the sample creates a filter to capture only content from the main display. To illustrate filtering a running app, the sample contains a toggle to specify whether to exclude the sample app from the stream.

```
```

### Create a stream configuration

An SCStreamConfiguration object provides properties to configure the stream’s output size, pixel format, audio capture settings, and more. The app’s configuration throttles frame updates to 60 fps, and configures the number of frames to keep in the queue at 5. Specifying more frames uses more memory, but may allow for processing frame data without stalling the display stream. The default value is 3 and shouldn’t exceed 8 frames.

```
```

### Start the capture session

The sample uses the content filter and stream configuration to initialize a new instance of SCStream. To retrieve audio and video sample data, the app adds stream outputs that capture media of the specified type. When the stream captures new sample buffers, it delivers them to its stream output object on the indicated dispatch queues.

```
```

After the stream starts, further changes to its configuration and content filter don’t require restarting it. Instead, after you update the capture configuration in the user interface, the sample creates new stream configuration and content filter objects and applies them to the running stream to update its state.

```
```

### Process the output

When a stream captures a new audio or video sample buffer, it calls the stream output’s stream(_:didOutputSampleBuffer:of:) method, passing it the captured data and an indicator of its type. The stream output evaluates and processes the sample buffer as shown below.

```
```

### Process a video sample buffer

If the sample buffer contains video data, it retrieves the sample buffer attachments that describe the output video frame.

```
```

An SCStreamFrameInfo structure defines dictionary keys that the sample uses to retrieve metadata attached to a sample buffer. Metadata includes information about the frame’s display time, scale factor, status, and more. To determine whether a frame is available for processing, the sample inspects the status for SCFrameStatus.complete.

```
```

The sample buffer wraps a CVPixelBuffer that’s backed by an IOSurface. The sample casts the surface reference to an `IOSurface` that it later sets as the layer content of an NSView.

```
```

### Process an audio sample buffer

If the sample buffer contains audio, it retrieves the data as an AudioBufferList as shown below.

```
```

The app retrieves the audio stream basic description that it uses to create an AVAudioFormat. It then uses the format and the audio buffer list to create a new instance of AVAudioPCMBuffer. If you enable audio capture in the user interface, the sample uses the buffer to calculate average levels for the captured audio to display in a simple level meter.

## See Also

### Essentials

ScreenCaptureKit updates

Learn about important changes to ScreenCaptureKit.

Persistent Content Capture

A Boolean value that indicates whether a Virtual Network Computing (VNC) app needs persistent access to screen capture.

