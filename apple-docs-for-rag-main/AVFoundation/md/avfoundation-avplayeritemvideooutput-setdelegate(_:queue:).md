

- AVFoundation
- AVPlayerItemVideoOutput
-  setDelegate(\_:queue:) 

Instance Method

# setDelegate(\_:queue:)

Sets the delegate and dispatch queue for the receiver.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func setDelegate(
    _ delegate: (any AVPlayerItemOutputPullDelegate)?,
    queue delegateQueue: dispatch_queue_t?
)
```

## Parameters 

`delegate`  

The delegate object for the receiver. You may specify `nil` for this parameter.

`delegateQueue`  

The dispatch queue on which to call delegate methods. If you specify `nil` for this parameter, the video output object calls the delegate on the dispatch queue for your app’s main thread.

## See Also

### Configuring the Delegate

var delegate: (any AVPlayerItemOutputPullDelegate)?

The delegate for the video output object.

protocol AVPlayerItemOutputPullDelegate

Methods you can implement to respond to pixel buffer changes.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which to call delegate methods.

