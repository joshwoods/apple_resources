

- AVFoundation
-  AVCaptureDepthDataOutputDelegate 

Protocol

# AVCaptureDepthDataOutputDelegate

Methods for receiving depth data produced by a depth capture output.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
protocol AVCaptureDepthDataOutputDelegate : NSObjectProtocol
```

## Topics

### Receiving Depth Data

func depthDataOutput(AVCaptureDepthDataOutput, didOutput: AVDepthData, timestamp: CMTime, connection: AVCaptureConnection)

Provides newly captured depth data to the delegate.

func depthDataOutput(AVCaptureDepthDataOutput, didDrop: AVDepthData, timestamp: CMTime, connection: AVCaptureConnection, reason: AVCaptureOutput.DataDroppedReason)

Informs the delegate that captured depth data was not processed.

enum DataDroppedReason

Constants that define reasons for why the system dropped a frame.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Receiving Captured Depth Data

func setDelegate((any AVCaptureDepthDataOutputDelegate)?, callbackQueue: dispatch_queue_t?)

Designates a delegate object to receive depth data and a dispatch queue for delivering that data.

var delegate: (any AVCaptureDepthDataOutputDelegate)?

A delegate object that receives depth data.

var delegateCallbackQueue: dispatch_queue_t?

A dispatch queue for delivering depth data.

