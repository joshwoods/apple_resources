

- ARKit
- ARSession
-  delegateQueue 

Instance Property

# delegateQueue

The dispatch queue through which the session calls your delegate methods.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var delegateQueue: dispatch_queue_t? { get set }
```

## Discussion

If this value is `nil` (the default), the session calls your delegate methods on the main queue.

## See Also

### Responding to events

var delegate: (any ARSessionDelegate)?

An object you provide to receive captured video images and tracking information, or to respond to changes in session status.

protocol ARSessionDelegate

Methods you can implement to receive captured video frame images and tracking state from an AR session.

protocol ARSessionObserver

Methods you can implement to respond to changes in the state of an AR session.

