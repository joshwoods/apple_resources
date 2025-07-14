

- Metal
- MTLRenderCommandEncoder
-  setScissorRects(\_:) 

Instance Method

# setScissorRects(\_:)

Configures multiple rectangles for the fragment scissor test.

iOS 12.0+iPadOS 12.0+Mac CatalystmacOS 10.13+tvOS 14.5+visionOS

``` source
func setScissorRects(_ scissorRects: [MTLScissorRect])
```

## Parameters 

`scissorRects`  

An array of MTLScissorRect instances the command applies to the render pipeline for clipping.

## Mentioned in 

Rendering to Multiple Viewports in a Draw Command

## Discussion

The rendering pipeline discards any fragments that lie outside the scissor rectangle. The default scissor rectangle is the same size as the current render attachment, with its origin coordinates in the upper-left corner at `(0, 0)`.

Use this method to configure a different scissor rectangle for multiple viewports you configure with the setViewports(_:) method. Multiple viewports give your app the ability to draw into separate areas of an image with a single draw call. You can either set a single scissor rectangle for all viewports with the setScissorRect(_:) method, or set each viewport’s rectangle with this method.

Important

The number of scissor rectangles you pass to this method needs to match the number of viewports you configure with the setViewports(_:) method.

The maximum number of viewports and scissor rectangles a GPU supports varies by device family. For more information, see MTLGPUFamily and Detecting GPU Features and Metal Software Versions.

The rendering pipeline sends each primitive to a single viewport and its associated scissor rectangle. You can select which viewport each primitive uses in your vertex shader by adding the `[[viewport_array_index]]` attribute to an output value.

Note

You can change the render pass’s scissor rectangle configuration by calling this method again or by calling the setScissorRect(_:) method.

The setScissorRect(_:) method is equivalent to calling this method with a single element in the `scissorRects` array.

## See Also

### Configuring Viewport and Scissor Behavior

func setViewport(MTLViewport)

Configures the render pipeline with a viewport that applies a transformation and a clipping rectangle.

**Required**

func setViewports([MTLViewport])

Configures the render pipeline with multiple viewports that apply transformations and clipping rectangles.

func setScissorRect(MTLScissorRect)

Configures a rectangle for the fragment scissor test.

**Required**

