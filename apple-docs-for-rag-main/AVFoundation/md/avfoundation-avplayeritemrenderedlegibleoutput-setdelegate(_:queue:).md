

- AVFoundation
- AVPlayerItemRenderedLegibleOutput
-  setDelegate(\_:queue:) 

Instance Method

# setDelegate(\_:queue:)

Sets the delegate object and the queue on which it’s invoked.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
func setDelegate(
    _ delegate: (any AVPlayerItemRenderedLegibleOutputPushDelegate)?,
    queue delegateQueue: dispatch_queue_t?
)
```

## Parameters 

`delegate`  

A delegate object for this output.

`delegateQueue`  

A dispatch queue on which the system calls all delegate methods.

## See Also

### Setting a delegate

var delegate: (any AVPlayerItemRenderedLegibleOutputPushDelegate)?

A delegate object for this output.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the output calls the delegate object.

protocol AVPlayerItemRenderedLegibleOutputPushDelegate

A delegate that handles the rendered pixel buffers produced by a rendered legible output object.

