

- AVFoundation
-  AVCaptureAudioDataOutputSampleBufferDelegate 

Protocol

# AVCaptureAudioDataOutputSampleBufferDelegate

Methods for receiving audio sample data from an audio capture.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
protocol AVCaptureAudioDataOutputSampleBufferDelegate : NSObjectProtocol
```

## Overview

This protocol defines an interface for delegates of an AVCaptureAudioDataOutput object to receive captured audio sample buffers.

The delegate of an AVCaptureAudioDataOutput object must adopt this protocol. The method in this protocol is optional.

## Topics

### Managing Sample Buffer Behavior

func captureOutput(AVCaptureOutput, didOutput: CMSampleBuffer, from: AVCaptureConnection)

Notifies the delegate that a sample buffer was written.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Receiving Captured Audio Data

func setSampleBufferDelegate((any AVCaptureAudioDataOutputSampleBufferDelegate)?, queue: dispatch_queue_t?)

Sets the delegate that will accept captured buffers and the dispatch queue on which the delegate will be called.

var sampleBufferDelegate: (any AVCaptureAudioDataOutputSampleBufferDelegate)?

The capture object’s delegate.

var sampleBufferCallbackQueue: dispatch_queue_t?

The queue on which delegate callbacks are invoked

