

- AVFoundation
-  AVCaptureScreenInput 

Class

# AVCaptureScreenInput

A capture input for recording from a screen in macOS.

macOS 10.7+

``` source
class AVCaptureScreenInput
```

## Overview

Important

Starting in macOS 12.3, use the ScreenCaptureKit framework for screen recording instead.

This class is a concrete capture input subclass that provides an interface to capture media from a screen or a portion of a screen.

Use instances of this class as input sources for AVCaptureSession objects that provide media data from one of the screens connected to the system, represented by CGDirectDisplayID.

## Topics

### Initializing a Capture Screen Input

init?(displayID: CGDirectDisplayID)

Initializes a capture screen input that provides media data from the specified display.

init()

Initializes a capture screen input that provides media data from the main screen.

### Setting Video Capture Options

var minFrameDuration: CMTime

The screen input’s minimum frame duration.

var cropRect: CGRect

Indicates the bounding rectangle of the screen area to be captured, in pixels.

var scaleFactor: CGFloat

Indicates the factor by which video buffers captured from the screen are to be scaled.

### Capturing Mouse Activity

var capturesCursor: Bool

A Boolean value that specifies whether the mouse cursor appears in the captured output.

var capturesMouseClicks: Bool

A Boolean value that specifies whether mouse clicks appear highlighted in the captured output.

### Deprecated

var removesDuplicateFrames: Bool

A Boolean value that specifies whether the capture input skips duplicate frames.

Deprecated

## Relationships

### Inherits From

- AVCaptureInput

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

