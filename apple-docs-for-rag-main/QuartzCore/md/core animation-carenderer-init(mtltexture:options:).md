

- Core Animation
- CARenderer
-  init(mtlTexture:options:) 

Initializer

# init(mtlTexture:options:)

Creates a layer renderer from a Metal texture.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init(
    mtlTexture tex: any MTLTexture,
    options dict: [AnyHashable : Any]? = nil
)
```

## See Also

### Creating a Renderer

init(cglContext: UnsafeMutableRawPointer, options: [AnyHashable : Any]?)

Creates and returns a `CARenderer` instance with the render target specified by the Core OpenGL context.

