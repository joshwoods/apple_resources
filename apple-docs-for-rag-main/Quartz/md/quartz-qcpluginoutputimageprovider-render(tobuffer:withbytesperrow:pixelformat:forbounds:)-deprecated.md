

- Quartz
- QCPlugInOutputImageProvider
-  render(toBuffer:withBytesPerRow:pixelFormat:forBounds:) Deprecated

Instance Method

# render(toBuffer:withBytesPerRow:pixelFormat:forBounds:)

Renders a subregion of the image into the supplied memory buffer using the specified pixel format.

macOS 10.4–10.15Deprecated

``` source
optional func render(
    toBuffer baseAddress: UnsafeMutableRawPointer!,
    withBytesPerRow rowBytes: Int,
    pixelFormat format: String!,
    forBounds bounds: NSRect
) -> Bool
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`baseAddress`  

The base address of the memory buffer. The Quartz Composer engine passes you an address that is aligned on a 16-byte boundary.

`rowBytes`  

The number of bytes per row of the image data. The Quartz Composer engine guarantees this value is a multiple of 16.

`format`  

The pixel format of the image data.

`bounds`  

The bounds of the subregion.

## Return Value

true if the image is rendered successfully into the buffer; false on failure or if the image provider doesn’t support CPU rendering.

## Discussion

The Quartz Composer engine calls this method when it needs pixels. It gives you the base address, the number of row bytes, and the format. Then, you write pixels to the buffer.

## See Also

### Rendering an Image to a Destination

func copyRenderedTexture(forCGLContext: CGLContextObj!, pixelFormat: String!, bounds: NSRect, isFlipped: UnsafeMutablePointer&lt;ObjCBool>!) -> GLuint

Returns the name of an OpenGL texture of type `GL_TEXTURE_RECTANGLE_EXT` that contains a subregion of the image in a given pixel format.

Deprecated

func render(withCGLContext: CGLContextObj!, forBounds: NSRect) -> Bool

Renders a subregion of the image to the provided CGL context.

Deprecated

func releaseRenderedTexture(GLuint, forCGLContext: CGLContextObj!)

Releases the previously copied texture.

Deprecated

