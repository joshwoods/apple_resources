

- AVFoundation
- AVPlayerItemLegibleOutput
-  advanceIntervalForDelegateInvocation 

Instance Property

# advanceIntervalForDelegateInvocation

The time interval, in seconds, that a player item legible output object messages its delegate earlier than normal.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var advanceIntervalForDelegateInvocation: TimeInterval { get set }
```

## Discussion

If possible, an `AVPlayerItemLegibleOutput` instance messages its delegate `advanceIntervalForDelegateInvocation` seconds earlier than it otherwise would.

If the value provided is large, the delegate methods are invoked as soon as possible.

## See Also

### Configuring the Delegate

var delegate: (any AVPlayerItemLegibleOutputPushDelegate)?

The delegate of the output class.

func setDelegate((any AVPlayerItemLegibleOutputPushDelegate)?, queue: dispatch_queue_t?)

Sets the receiver’s delegate and a dispatch queue on which the delegate is called.

protocol AVPlayerItemLegibleOutputPushDelegate

Methods you can implement to provide alternative attributed-string output.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the delegate is called.

