

- AVFoundation
- AVPlayerItemMetadataOutput
-  setDelegate(\_:queue:) 

Instance Method

# setDelegate(\_:queue:)

Sets the delegate and a dispatch queue on which the delegate is called.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func setDelegate(
    _ delegate: (any AVPlayerItemMetadataOutputPushDelegate)?,
    queue delegateQueue: dispatch_queue_t?
)
```

## Parameters 

`delegate`  

An object conforming to AVPlayerItemMetadataOutputPushDelegate protocol.

`delegateQueue`  

A dispatch queue on which all delegate methods will be called.

## Discussion

You specify the metadata delegate, and a dispatch queue on which it will be called, to be notified as new metadata is encountered in the source media.

Important

The values set for the `delegate` and `delegateQueue` arguments can be `nil` , but passing `nil` for one requires you to do the same for the other. Passing a `nil` value for only one argument results in an exception being raised at runtime.

## See Also

### Configuring the Delegate

var advanceIntervalForDelegateInvocation: TimeInterval

The time interval, in seconds, the player item metadata output object messages its delegate earlier than normal.

var delegate: (any AVPlayerItemMetadataOutputPushDelegate)?

The delegate object.

protocol AVPlayerItemMetadataOutputPushDelegate

Methods you can implement to provide additional metadata.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which messages are sent to the delegate.

