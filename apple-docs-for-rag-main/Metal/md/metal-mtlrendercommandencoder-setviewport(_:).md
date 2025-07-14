

- Metal
- MTLRenderCommandEncoder
-  setViewport(\_:) 

Instance Method

# setViewport(\_:)

Configures the render pipeline with a viewport that applies a transformation and a clipping rectangle.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func setViewport(_ viewport: MTLViewport)
```

**Required**

## Parameters 

`viewport`  

An MTLViewport instance the command applies to the render pipeline for transformations and clipping.

## Discussion

The render pipeline linearly maps vertex positions from normalized device coordinates to viewport coordinates by applying a viewport during the rasterization stage. It applies the transform first and then rasterizes the primitive while clipping any fragments outside the scissor rectangle (see setScissorRect(_:)) or the render target’s extents.

The viewport’s originX and originY properties, which default to `0.0`, represent the number of pixels from the top-left corner of the render target. Positive originX values go to the right and positive originY values go downward. The default values for its width and height properties are the render target’s width and height, respectively. The default values for its znear and zfar properties are `0.0` and `1.0`, respectively, which you can flip.

Note

You can change the render pass’s viewport configuration by calling this method again, or by calling the setViewports(_:) method.

## See Also

### Configuring Viewport and Scissor Behavior

func setViewports([MTLViewport])

Configures the render pipeline with multiple viewports that apply transformations and clipping rectangles.

func setScissorRect(MTLScissorRect)

Configures a rectangle for the fragment scissor test.

**Required**

func setScissorRects([MTLScissorRect])

Configures multiple rectangles for the fragment scissor test.

