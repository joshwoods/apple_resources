

- Quartz
- QCPlugInOutputImageProvider
-  copyRenderedTexture(forCGLContext:pixelFormat:bounds:isFlipped:) Deprecated

Instance Method

# copyRenderedTexture(forCGLContext:pixelFormat:bounds:isFlipped:)

Returns the name of an OpenGL texture of type `GL_TEXTURE_RECTANGLE_EXT` that contains a subregion of the image in a given pixel format.

macOS 10.5–10.14Deprecated

``` source
optional func copyRenderedTexture(
    forCGLContext cgl_ctx: CGLContextObj!,
    pixelFormat format: String!,
    bounds: NSRect,
    isFlipped flipped: UnsafeMutablePointer!
) -> GLuint
```

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`cgl_ctx`  

The CGL context to render to.

`format`  

A string that represents the pixel format of the texture.

`bounds`  

The bounds of the subregion of the image.

`flipped`  

Set to true on output if the contents of the returned texture are vertically flipped.

## Return Value

The name of an OpenGL texture of type `GL_TEXTURE_RECTANGLE_EXT` that contains a subregion of the image in a given pixel format or `0` if the texture can’t be provided.

## Discussion

Implement this method if you want to create the texture yourself or use framebuffer objects (FBO). Use `` to send commands to the OpenGL context. Make sure to preserve all the OpenGL states except the ones defined by `GL_CURRENT_BIT`.

## See Also

### Rendering an Image to a Destination

func render(toBuffer: UnsafeMutableRawPointer!, withBytesPerRow: Int, pixelFormat: String!, forBounds: NSRect) -> Bool

Renders a subregion of the image into the supplied memory buffer using the specified pixel format.

Deprecated

func render(withCGLContext: CGLContextObj!, forBounds: NSRect) -> Bool

Renders a subregion of the image to the provided CGL context.

Deprecated

func releaseRenderedTexture(GLuint, forCGLContext: CGLContextObj!)

Releases the previously copied texture.

Deprecated

