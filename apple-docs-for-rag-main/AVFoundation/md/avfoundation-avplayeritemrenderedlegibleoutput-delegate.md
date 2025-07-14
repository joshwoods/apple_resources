

- AVFoundation
- AVPlayerItemRenderedLegibleOutput
-  delegate 

Instance Property

# delegate

A delegate object for this output.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
weak var delegate: (any AVPlayerItemRenderedLegibleOutputPushDelegate)? { get }
```

## See Also

### Setting a delegate

func setDelegate((any AVPlayerItemRenderedLegibleOutputPushDelegate)?, queue: dispatch_queue_t?)

Sets the delegate object and the queue on which it’s invoked.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the output calls the delegate object.

protocol AVPlayerItemRenderedLegibleOutputPushDelegate

A delegate that handles the rendered pixel buffers produced by a rendered legible output object.

