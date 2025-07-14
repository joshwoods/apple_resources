

- SceneKit
- SCNSceneRenderer
-  device 

Instance Property

# device

The Metal device this renderer uses for rendering.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var device: (any MTLDevice)? { get }
```

**Required**

## Discussion

Use this property to create or look up other Metal resources that use the same device as your SceneKit renderer.

Note

This property is valid only for scene renderers whose renderingAPI value is SCNRenderingAPI.metal. You create a SceneKit view that renders using Metal with the preferredRenderingAPI initialization option or in Interface Builder, or an SCNRenderer that uses Metal with the init(device:options:) method. For OpenGL-based scene renderers, this property’s value is always `nil`.

## See Also

### Customizing Scene Rendering with Metal

var currentRenderCommandEncoder: (any MTLRenderCommandEncoder)?

The Metal render command encoder in use for the current SceneKit rendering pass.

**Required**

var commandQueue: (any MTLCommandQueue)?

The Metal command queue this renderer uses for rendering.

**Required**

var colorPixelFormat: MTLPixelFormat

The Metal pixel format for the renderer’s color output.

**Required**

var depthPixelFormat: MTLPixelFormat

The Metal pixel format for the renderer’s depth buffer.

**Required**

var stencilPixelFormat: MTLPixelFormat

The Metal pixel format for the renderer’s stencil buffer.

**Required**

