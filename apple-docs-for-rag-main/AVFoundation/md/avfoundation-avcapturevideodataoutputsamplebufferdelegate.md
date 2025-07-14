

- AVFoundation
-  AVCaptureVideoDataOutputSampleBufferDelegate 

Protocol

# AVCaptureVideoDataOutputSampleBufferDelegate

Methods for receiving sample buffers from, and monitoring the status of, a video data output.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
protocol AVCaptureVideoDataOutputSampleBufferDelegate : NSObjectProtocol
```

## Overview

This protocol defines an interface for delegates of an AVCaptureVideoDataOutput object to receive captured video sample buffers and be notified of late sample buffers that were dropped.

The delegate of an AVCaptureVideoDataOutput object must adopt the `AVCaptureVideoDataOutputSampleBufferDelegate` protocol. The methods in this protocol are optional.

## Topics

### Managing Sample Buffer Behavior

func captureOutput(AVCaptureOutput, didOutput: CMSampleBuffer, from: AVCaptureConnection)

Notifies the delegate that a new video frame was written.

func captureOutput(AVCaptureOutput, didDrop: CMSampleBuffer, from: AVCaptureConnection)

Notifies the delegate that a video frame was discarded.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Receiving Captured Video Data

func setSampleBufferDelegate((any AVCaptureVideoDataOutputSampleBufferDelegate)?, queue: dispatch_queue_t?)

Sets the sample buffer delegate and the queue for invoking callbacks.

var sampleBufferDelegate: (any AVCaptureVideoDataOutputSampleBufferDelegate)?

The capture object’s delegate.

var sampleBufferCallbackQueue: dispatch_queue_t?

The queue on which the system invokes delegate callbacks.

