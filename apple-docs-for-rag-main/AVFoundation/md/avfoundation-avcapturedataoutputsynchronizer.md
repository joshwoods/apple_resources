

- AVFoundation
-  AVCaptureDataOutputSynchronizer 

Class

# AVCaptureDataOutputSynchronizer

An object that coordinates time-matched delivery of data from multiple capture outputs.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
class AVCaptureDataOutputSynchronizer
```

## Overview

Use this class when you need to capture media from multiple capture outputs and want to receive all data samples from the same timestamp in a single delegate callback.

For example, when you use an AVCaptureDataOutputSynchronizer object to coordinate the output of AVCaptureVideoDataOutput and AVCaptureDepthDataOutput objects, you can easily match each captured video frame to depth information captured at the same moment.

## Topics

### Configuring Synchronized Capture

init(dataOutputs: [AVCaptureOutput])

Creates a capture output synchronizer for the specified capture outputs.

var dataOutputs: [AVCaptureOutput]

The list of data outputs governed by this data output synchronizer.

### Receiving Synchronized Capture Data

func setDelegate((any AVCaptureDataOutputSynchronizerDelegate)?, queue: dispatch_queue_t?)

Designates a delegate object to receive synchronized data and a dispatch queue for delivering that data.

var delegate: (any AVCaptureDataOutputSynchronizerDelegate)?

A delegate object that receives synchronized capture data.

var delegateCallbackQueue: dispatch_queue_t?

A dispatch queue for delivering synchronized capture data.

protocol AVCaptureDataOutputSynchronizerDelegate

Methods for receiving captured data from multiple capture outputs synchronized to the same timestamp.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Synchronized capture

class AVCaptureSynchronizedDataCollection

A set of data samples collected simultaneously from multiple capture outputs.

class AVCaptureSynchronizedSampleBufferData

A container for video or audio samples collected using synchronized capture.

class AVCaptureSynchronizedMetadataObjectData

A container for metadata objects collected using synchronized capture.

class AVCaptureSynchronizedDepthData

A container for scene depth information collected using synchronized capture.

class AVCaptureSynchronizedData

The abstract superclass for media samples collected using synchronized capture.

