

- MetalKit
- MTKView
-  currentDrawable 

Instance Property

# currentDrawable

The drawable to use for the current frame.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var currentDrawable: (any CAMetalDrawable)? { get }
```

## Discussion

If all drawable objects are in use, the value of this property is `nil`. Your app should check that currentDrawable isn’t `nil` before attempting to draw. The view changes the value of this property only after returning from a drawing function, either draw(_:) from a subclassed instance of the view, or draw(in:) from the view’s delegate.

Use a MTLRenderCommandEncoder object to render into the drawable’s texture and present it for display (typically registered using the present(_:) method of a command buffer). Try to minimize the time between when you fetch the drawable and when you submit the command buffer that uses it. For more information, see CAMetalLayer.

## See Also

### Retrieving Render Target Information

var currentRenderPassDescriptor: MTLRenderPassDescriptor?

A render pass descriptor to draw into the current drawable.

var depthStencilTexture: (any MTLTexture)?

A packed depth and stencil texture associated with the current drawable object’s texture.

var depthStencilStorageMode: MTLStorageMode

The storage mode that the packed depth and stencil texture use.

var multisampleColorTexture: (any MTLTexture)?

The multisample color sample texture to render into.

