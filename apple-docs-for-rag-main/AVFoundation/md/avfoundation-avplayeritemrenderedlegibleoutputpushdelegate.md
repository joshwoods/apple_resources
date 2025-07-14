

- AVFoundation
-  AVPlayerItemRenderedLegibleOutputPushDelegate 

Protocol

# AVPlayerItemRenderedLegibleOutputPushDelegate

A delegate that handles the rendered pixel buffers produced by a rendered legible output object.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
protocol AVPlayerItemRenderedLegibleOutputPushDelegate : AVPlayerItemOutputPushDelegate
```

## Topics

### Handling rendered pixel buffers

func renderedLegibleOutput(AVPlayerItemRenderedLegibleOutput, didOutputRenderedCaptionImages: [AVRenderedCaptionImage], forItemTime: CMTime)

Tells the delegate that new rendered caption images are available.

## Relationships

### Inherits From

- AVPlayerItemOutputPushDelegate
- NSObjectProtocol
- Sendable

## See Also

### Setting a delegate

var delegate: (any AVPlayerItemRenderedLegibleOutputPushDelegate)?

A delegate object for this output.

func setDelegate((any AVPlayerItemRenderedLegibleOutputPushDelegate)?, queue: dispatch_queue_t?)

Sets the delegate object and the queue on which it’s invoked.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the output calls the delegate object.

