

- AVFoundation
-  AVCaptureDataOutputSynchronizerDelegate 

Protocol

# AVCaptureDataOutputSynchronizerDelegate

Methods for receiving captured data from multiple capture outputs synchronized to the same timestamp.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
protocol AVCaptureDataOutputSynchronizerDelegate : NSObjectProtocol
```

## Topics

### Receiving Synchronized Capture Data

func dataOutputSynchronizer(AVCaptureDataOutputSynchronizer, didOutput: AVCaptureSynchronizedDataCollection)

Provides a collection of synchronized capture data to the delegate.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Receiving Synchronized Capture Data

func setDelegate((any AVCaptureDataOutputSynchronizerDelegate)?, queue: dispatch_queue_t?)

Designates a delegate object to receive synchronized data and a dispatch queue for delivering that data.

var delegate: (any AVCaptureDataOutputSynchronizerDelegate)?

A delegate object that receives synchronized capture data.

var delegateCallbackQueue: dispatch_queue_t?

A dispatch queue for delivering synchronized capture data.

