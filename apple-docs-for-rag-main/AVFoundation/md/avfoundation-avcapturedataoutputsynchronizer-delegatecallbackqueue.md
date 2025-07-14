

- AVFoundation
- AVCaptureDataOutputSynchronizer
-  delegateCallbackQueue 

Instance Property

# delegateCallbackQueue

A dispatch queue for delivering synchronized capture data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var delegateCallbackQueue: dispatch_queue_t? { get }
```

## Discussion

This property is read-only. You set the delegate object and the dispatch queue for delegate methods together using the setDelegate(_:queue:) method.

## See Also

### Receiving Synchronized Capture Data

func setDelegate((any AVCaptureDataOutputSynchronizerDelegate)?, queue: dispatch_queue_t?)

Designates a delegate object to receive synchronized data and a dispatch queue for delivering that data.

var delegate: (any AVCaptureDataOutputSynchronizerDelegate)?

A delegate object that receives synchronized capture data.

protocol AVCaptureDataOutputSynchronizerDelegate

Methods for receiving captured data from multiple capture outputs synchronized to the same timestamp.

