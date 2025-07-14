

- Metal
- MTLRenderCommandEncoder
-  setScissorRect(\_:) 

Instance Method

# setScissorRect(\_:)

Configures a rectangle for the fragment scissor test.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setScissorRect(_ rect: MTLScissorRect)
```

**Required**

## Parameters 

`rect`  

An MTLScissorRect instance that represents a rectangle that needs to lie completely within the current render attachment.

## Discussion

The rendering pipeline discards any fragments that lie outside the scissor rectangle.

The default scissor rectangle is the same size as the current render attachment, with its origin coordinates in the upper-left corner at `(0, 0)`.

Note

You can change the render pass’s scissor rectangle configuration by calling this method again or by calling the setScissorRects(_:) method.

## See Also

### Configuring Viewport and Scissor Behavior

func setViewport(MTLViewport)

Configures the render pipeline with a viewport that applies a transformation and a clipping rectangle.

**Required**

func setViewports([MTLViewport])

Configures the render pipeline with multiple viewports that apply transformations and clipping rectangles.

func setScissorRects([MTLScissorRect])

Configures multiple rectangles for the fragment scissor test.

