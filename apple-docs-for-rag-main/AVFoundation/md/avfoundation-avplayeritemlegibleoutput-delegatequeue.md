

- AVFoundation
- AVPlayerItemLegibleOutput
-  delegateQueue 

Instance Property

# delegateQueue

The dispatch queue on which the delegate is called.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var delegateQueue: dispatch_queue_t? { get }
```

## Discussion

This property does not support key-value observing.

## See Also

### Configuring the Delegate

var delegate: (any AVPlayerItemLegibleOutputPushDelegate)?

The delegate of the output class.

func setDelegate((any AVPlayerItemLegibleOutputPushDelegate)?, queue: dispatch_queue_t?)

Sets the receiver’s delegate and a dispatch queue on which the delegate is called.

protocol AVPlayerItemLegibleOutputPushDelegate

Methods you can implement to provide alternative attributed-string output.

var advanceIntervalForDelegateInvocation: TimeInterval

The time interval, in seconds, that a player item legible output object messages its delegate earlier than normal.

