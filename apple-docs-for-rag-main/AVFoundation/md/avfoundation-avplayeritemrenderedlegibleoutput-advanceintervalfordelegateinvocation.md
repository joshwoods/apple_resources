

- AVFoundation
- AVPlayerItemRenderedLegibleOutput
-  advanceIntervalForDelegateInvocation 

Instance Property

# advanceIntervalForDelegateInvocation

Permits advance invocation of the associated delegate, if any.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var advanceIntervalForDelegateInvocation: TimeInterval { get set }
```

## Discussion

Use this property specify the number of seconds early to invoke the delegate object. When possible, an AVPlayerItemLegibleOutput uses this value to call its delegate earlier than it would otherwise.

## See Also

### Configuring an output

var videoDisplaySize: CGSize

Set the video display size to use for rendering of pixel buffers.

