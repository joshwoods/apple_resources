

- ScreenCaptureKit
-  SCStreamOutput 

Protocol

# SCStreamOutput

A delegate protocol your app implements to receive capture stream output events.

Mac Catalyst 18.2+macOS 12.3+

``` source
protocol SCStreamOutput : NSObjectProtocol
```

## Overview

The SCStreamOutput protocol provides a way to retrieve output from an SCStream.

After you call startCapture(completionHandler:), the system provides frame data through the stream(_:didOutputSampleBuffer:of:) method. You can inspect the CMSampleBuffer to retrieve image data, and inspect the sample buffer for metadata about the frame.

## Topics

### Receiving stream output

func stream(SCStream, didOutputSampleBuffer: CMSampleBuffer, of: SCStreamOutputType)

Tells the delegate that a capture stream produced a frame.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Output processing

enum SCStreamOutputType

Constants that represent output types for a stream frame.

struct SCStreamFrameInfo

An instance that defines metadata keys for a stream frame.

enum SCFrameStatus

Status values for a frame from a stream.

