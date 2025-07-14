

- Quartz
- QCPlugInInputImageSource
-  bindTextureRepresentation(toCGLContext:textureUnit:normalizeCoordinates:) Deprecated

Instance Method

# bindTextureRepresentation(toCGLContext:textureUnit:normalizeCoordinates:)

Binds the texture to a given texture unit and optionally scales or flips the texture.

macOS 10.5–10.14Deprecated

``` source
func bindTextureRepresentation(
    toCGLContext cgl_ctx: CGLContextObj!,
    textureUnit unit: GLenum,
    normalizeCoordinates flag: Bool
)
```

**Required**

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`cgl_ctx`  

The CGL context to render to.)

`unit`  

The texture unit to bind to (such as, `GL_TEXTURE0`)

`flag`  

To apply a texture matrix to scale coordinates (from `[0, pixels]` to `[0,1]`) and flip them vertically (if necessary), pass true.

## Discussion

When you no longer need the texture, call unbindTextureRepresentation(fromCGLContext:textureUnit:).

## See Also

### Converting an Image to a Representation

func lockTextureRepresentation(with: CGColorSpace!, forBounds: NSRect) -> Bool

Creates an OpenGL texture representation from a subregion of the image source using the provided color space.

**Required**

Deprecated

func unlockTextureRepresentation()

Releases the OpenGL texture representation of the image source.

**Required**

Deprecated

func lockBufferRepresentation(withPixelFormat: String!, colorSpace: CGColorSpace!, forBounds: NSRect) -> Bool

Creates a memory buffer representation from a subregion of the image source using the provided pixel format and color space.

**Required**

Deprecated

func unbindTextureRepresentation(fromCGLContext: CGLContextObj!, textureUnit: GLenum)

Unbinds the texture from a texture unit.

**Required**

Deprecated

func unlockBufferRepresentation()

Releases the memory buffer representation of the image source.

**Required**

Deprecated

