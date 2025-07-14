

- Quartz
- QCPlugInOutputImageProvider
-  render(withCGLContext:forBounds:) Deprecated

Instance Method

# render(withCGLContext:forBounds:)

Renders a subregion of the image to the provided CGL context.

macOS 10.5–10.14Deprecated

``` source
optional func render(
    withCGLContext cgl_ctx: CGLContextObj!,
    forBounds bounds: NSRect
) -> Bool
```

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`cgl_ctx`  

The CGL context to render to.

`bounds`  

The bounds of the subregion.

## Return Value

true if successful; false on failure or if the image provider doesn’t support GPU rendering.

## Discussion

The view port is set for you. The model view and projection matrixes are set to the identity.

Your OpenGL code should save and restore all states *except* for those that are part of `GL_CURRENT_BIT` (vertex position, color, texture, and so on). Also use CGL macros instead of changing the current context, by including this statement:

`#import `

For more details, see Quartz Composer Custom Patch Programming Guide.

## See Also

### Rendering an Image to a Destination

func render(toBuffer: UnsafeMutableRawPointer!, withBytesPerRow: Int, pixelFormat: String!, forBounds: NSRect) -> Bool

Renders a subregion of the image into the supplied memory buffer using the specified pixel format.

Deprecated

func copyRenderedTexture(forCGLContext: CGLContextObj!, pixelFormat: String!, bounds: NSRect, isFlipped: UnsafeMutablePointer&lt;ObjCBool>!) -> GLuint

Returns the name of an OpenGL texture of type `GL_TEXTURE_RECTANGLE_EXT` that contains a subregion of the image in a given pixel format.

Deprecated

func releaseRenderedTexture(GLuint, forCGLContext: CGLContextObj!)

Releases the previously copied texture.

Deprecated

