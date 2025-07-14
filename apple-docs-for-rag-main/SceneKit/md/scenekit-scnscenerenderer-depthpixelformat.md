

- SceneKit
- SCNSceneRenderer
-  depthPixelFormat 

Instance Property

# depthPixelFormat

The Metal pixel format for the renderer’s depth buffer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var depthPixelFormat: MTLPixelFormat { get }
```

**Required**

## Discussion

Use this property, along with the colorPixelFormat and stencilPixelFormat properties, if you perform custom drawing with Metal (see the SCNSceneRendererDelegate and SCNNodeRendererDelegate classes) and need to create a new MTLRenderPipelineState object to change the GPU state as part of your rendering.

Note

This property is valid only for scene renderers whose renderingAPI value is SCNRenderingAPI.metal. You create a SceneKit view that renders using Metal with the preferredRenderingAPI initialization option or in Interface Builder, or an SCNRenderer that uses Metal with the init(device:options:) method. For OpenGL-based scene renderers, this property’s value is always `nil`.

## See Also

### Customizing Scene Rendering with Metal

var currentRenderCommandEncoder: (any MTLRenderCommandEncoder)?

The Metal render command encoder in use for the current SceneKit rendering pass.

**Required**

var device: (any MTLDevice)?

The Metal device this renderer uses for rendering.

**Required**

var commandQueue: (any MTLCommandQueue)?

The Metal command queue this renderer uses for rendering.

**Required**

var colorPixelFormat: MTLPixelFormat

The Metal pixel format for the renderer’s color output.

**Required**

var stencilPixelFormat: MTLPixelFormat

The Metal pixel format for the renderer’s stencil buffer.

**Required**

