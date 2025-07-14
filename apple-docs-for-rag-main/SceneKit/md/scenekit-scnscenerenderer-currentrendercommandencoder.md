

- SceneKit
- SCNSceneRenderer
-  currentRenderCommandEncoder 

Instance Property

# currentRenderCommandEncoder

The Metal render command encoder in use for the current SceneKit rendering pass.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var currentRenderCommandEncoder: (any MTLRenderCommandEncoder)? { get }
```

**Required**

## Discussion

Use this render command encoder to encode additional rendering commands before or after SceneKit draws its own content.

This property is valid only during the SceneKit rendering loop—that is, within one of the methods defined in the SCNSceneRendererDelegate protocol. Accessing this property at any other time returns `nil`.

## See Also

### Customizing Scene Rendering with Metal

var device: (any MTLDevice)?

The Metal device this renderer uses for rendering.

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

