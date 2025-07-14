

- AVFoundation
- AVCaptureDepthDataOutput
-  setDelegate(\_:callbackQueue:) 

Instance Method

# setDelegate(\_:callbackQueue:)

Designates a delegate object to receive depth data and a dispatch queue for delivering that data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func setDelegate(
    _ delegate: (any AVCaptureDepthDataOutputDelegate)?,
    callbackQueue: dispatch_queue_t?
)
```

## Parameters 

`delegate`  

A delegate object to receive depth data.

`callbackQueue`  

The dispatch queue on which to call delegate methods. This parameter must be a serial dispatch queue to guarantee that depth data is delivered in order.

## Discussion

The depth data output vends captured depth data by calling delegate methods on the specified dispatch queue.

If the callback queue is blocked when new depth data is captured, the alwaysDiscardsLateDepthData property determines whether to discard data or hold it for later delivery, allowing you to choose whether to prioritize timeliness or memory usage when your processing is unable to keep up with the rate of incoming depth data.

If you need to minimize the chances of depth data being dropped, provide a dedicated queue and do not share it with other data outputs. The capture output can defer processing of depth data to another queue; however, depth data pixel buffer maps may come from a finite buffer pool, which may be starved if your deferred processing fails to keep up.

## See Also

### Receiving Captured Depth Data

var delegate: (any AVCaptureDepthDataOutputDelegate)?

A delegate object that receives depth data.

var delegateCallbackQueue: dispatch_queue_t?

A dispatch queue for delivering depth data.

protocol AVCaptureDepthDataOutputDelegate

Methods for receiving depth data produced by a depth capture output.

