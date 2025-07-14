

- MetalKit
- MTKView
-  currentRenderPassDescriptor 

Instance Property

# currentRenderPassDescriptor

A render pass descriptor to draw into the current drawable.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var currentRenderPassDescriptor: MTLRenderPassDescriptor? { get }
```

## Discussion

Reading this property creates and returns a new render pass descriptor to render into the current drawable’s texture. MTKView doesn’t use this descriptor, and there’s no requirement for your application to use it.

This property is `nil` if the view’s device property isn’t set or if currentDrawable is `nil`. Your app should check that currentRenderPassDescriptor isn’t `nil` before attempting to use it.

The view configures the render pass as follows:

- If multisampling isn’t enabled—The color attachment at index 0 of the render pass descriptor points to the texture assigned to the current drawable, with a load action of MTLLoadAction.clear and a store action of MTLStoreAction.store.

- If you’ve enabled multisampling—The color attachment at index 0 of the render pass descriptor points to the multisample texture, the resolve texture points to the texture assigned to the current drawable, and the attachment has a load action of MTLLoadAction.clear and a store action of MTLStoreAction.multisampleResolve.

- If you’ve specified a depth or stencil target—The render pass configures the appropriate targets, with a load action of MTLLoadAction.clear and a store action of MTLStoreAction.dontCare.

## See Also

### Retrieving Render Target Information

var currentDrawable: (any CAMetalDrawable)?

The drawable to use for the current frame.

var depthStencilTexture: (any MTLTexture)?

A packed depth and stencil texture associated with the current drawable object’s texture.

var depthStencilStorageMode: MTLStorageMode

The storage mode that the packed depth and stencil texture use.

var multisampleColorTexture: (any MTLTexture)?

The multisample color sample texture to render into.

