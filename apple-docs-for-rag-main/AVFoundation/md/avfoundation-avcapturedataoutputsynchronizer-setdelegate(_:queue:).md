

- AVFoundation
- AVCaptureDataOutputSynchronizer
-  setDelegate(\_:queue:) 

Instance Method

# setDelegate(\_:queue:)

Designates a delegate object to receive synchronized data and a dispatch queue for delivering that data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
func setDelegate(
    _ delegate: (any AVCaptureDataOutputSynchronizerDelegate)?,
    queue delegateCallbackQueue: dispatch_queue_t?
)
```

## Parameters 

`delegate`  

A delegate object to receive synchronized data.

`delegateCallbackQueue`  

The dispatch queue on which to call delegate methods. This parameter must be a serial dispatch queue to guarantee that captured data is delivered in order.

## Discussion

The data output synchronizer gathers data from its data outputs, and when it determines that all data has been received for a given timestamp, it vends collections of synchronized data by calling delegate methods on the specified dispatch queue.

The AVCaptureDataOutputSynchronizer class overrides all the data outputs’ own delegates and callbacks. Data outputs under the control of a data output synchronizer do not fire delegate callbacks. Delegate callbacks are restored to individual data outputs only if you clear the synchronizer’s delegate and callback queue by calling this method and passing `nil` for both parameters.

## See Also

### Receiving Synchronized Capture Data

var delegate: (any AVCaptureDataOutputSynchronizerDelegate)?

A delegate object that receives synchronized capture data.

var delegateCallbackQueue: dispatch_queue_t?

A dispatch queue for delivering synchronized capture data.

protocol AVCaptureDataOutputSynchronizerDelegate

Methods for receiving captured data from multiple capture outputs synchronized to the same timestamp.

