

- AVFoundation
- AVCaptureDepthDataOutput
-  delegateCallbackQueue 

Instance Property

# delegateCallbackQueue

A dispatch queue for delivering depth data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var delegateCallbackQueue: dispatch_queue_t? { get }
```

## Discussion

This property is read-only. You set the delegate object and the dispatch queue for calling delegate methods together using the setDelegate(_:callbackQueue:) method.

## See Also

### Receiving Captured Depth Data

func setDelegate((any AVCaptureDepthDataOutputDelegate)?, callbackQueue: dispatch_queue_t?)

Designates a delegate object to receive depth data and a dispatch queue for delivering that data.

var delegate: (any AVCaptureDepthDataOutputDelegate)?

A delegate object that receives depth data.

protocol AVCaptureDepthDataOutputDelegate

Methods for receiving depth data produced by a depth capture output.

