

- AVFoundation
- AVPlayerItemLegibleOutput
-  setDelegate(\_:queue:) 

Instance Method

# setDelegate(\_:queue:)

Sets the receiver’s delegate and a dispatch queue on which the delegate is called.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func setDelegate(
    _ delegate: (any AVPlayerItemLegibleOutputPushDelegate)?,
    queue delegateQueue: dispatch_queue_t?
)
```

## Parameters 

`delegate`  

An object conforming to the AVPlayerItemLegibleOutputPushDelegate protocol.

`delegateQueue`  

A dispatch queue on which all delegate methods will be called.

## Discussion

Because the delegate is held using a zeroing-weak reference, it is safe to deallocate the delegate while the receiver still has a reference to it.

## See Also

### Configuring the Delegate

var delegate: (any AVPlayerItemLegibleOutputPushDelegate)?

The delegate of the output class.

protocol AVPlayerItemLegibleOutputPushDelegate

Methods you can implement to provide alternative attributed-string output.

var advanceIntervalForDelegateInvocation: TimeInterval

The time interval, in seconds, that a player item legible output object messages its delegate earlier than normal.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the delegate is called.

