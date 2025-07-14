

- AVFoundation
- AVVideoCompositing
-  renderContextChanged(\_:) 

Instance Method

# renderContextChanged(\_:)

Tells the compositor that the composition changed render contexts.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func renderContextChanged(_ newRenderContext: AVVideoCompositionRenderContext)
```

**Required**

## Parameters 

`newRenderContext`  

The new render context of the video composition.

## See Also

### Observing Render Context Changes

class AVVideoCompositionRenderContext

An object that defines the context in which custom compositors render pixel buffers.

