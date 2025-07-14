

- Core Animation
- CARenderer
-  init(cglContext:options:) 

Initializer

# init(cglContext:options:)

Creates and returns a `CARenderer` instance with the render target specified by the Core OpenGL context.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1–13.1DeprecatedmacOS 10.5–10.14Deprecated

``` source
init(
    cglContext ctx: UnsafeMutableRawPointer,
    options dict: [AnyHashable : Any]? = nil
)
```

## Parameters 

`ctx`  

A Core OpenGL render context that is used as the render target.

`dict`  

A dictionary of optional parameters.

## Return Value

A new instance of `CARenderer` that will use `ctx` as the render target.

## See Also

### Creating a Renderer

init(mtlTexture: any MTLTexture, options: [AnyHashable : Any]?)

Creates a layer renderer from a Metal texture.

