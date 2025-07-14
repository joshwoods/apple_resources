

- AVFoundation
- AVPlayerItemLegibleOutput
-  delegate 

Instance Property

# delegate

The delegate of the output class.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
weak var delegate: (any AVPlayerItemLegibleOutputPushDelegate)? { get }
```

## Discussion

Because the delegate is held using a zeroing-weak reference, this property has a value of `nil` after a delegate that was previously set has been deallocated.

This property does not support key-value observing.

## See Also

### Configuring the Delegate

func setDelegate((any AVPlayerItemLegibleOutputPushDelegate)?, queue: dispatch_queue_t?)

Sets the receiver’s delegate and a dispatch queue on which the delegate is called.

protocol AVPlayerItemLegibleOutputPushDelegate

Methods you can implement to provide alternative attributed-string output.

var advanceIntervalForDelegateInvocation: TimeInterval

The time interval, in seconds, that a player item legible output object messages its delegate earlier than normal.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the delegate is called.

