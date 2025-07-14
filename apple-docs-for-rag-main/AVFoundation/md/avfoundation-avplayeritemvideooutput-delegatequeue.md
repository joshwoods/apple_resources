

- AVFoundation
- AVPlayerItemVideoOutput
-  delegateQueue 

Instance Property

# delegateQueue

The dispatch queue on which to call delegate methods.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
var delegateQueue: dispatch_queue_t? { get }
```

## See Also

### Configuring the Delegate

func setDelegate((any AVPlayerItemOutputPullDelegate)?, queue: dispatch_queue_t?)

Sets the delegate and dispatch queue for the receiver.

var delegate: (any AVPlayerItemOutputPullDelegate)?

The delegate for the video output object.

protocol AVPlayerItemOutputPullDelegate

Methods you can implement to respond to pixel buffer changes.

