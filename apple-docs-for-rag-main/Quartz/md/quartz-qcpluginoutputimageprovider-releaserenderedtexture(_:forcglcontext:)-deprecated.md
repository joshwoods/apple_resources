

- Quartz
- QCPlugInOutputImageProvider
-  releaseRenderedTexture(\_:forCGLContext:) Deprecated

Instance Method

# releaseRenderedTexture(\_:forCGLContext:)

Releases the previously copied texture.

macOS 10.5–10.14Deprecated

``` source
optional func releaseRenderedTexture(
    _ name: GLuint,
    forCGLContext cgl_ctx: CGLContextObj!
)
```

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`name`  

The name of the previously bound texture.

`cgl_ctx`  

The CGL context.

## Discussion

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

func render(withCGLContext: CGLContextObj!, forBounds: NSRect) -> Bool

Renders a subregion of the image to the provided CGL context.

Deprecated

