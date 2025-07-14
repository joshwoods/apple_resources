

- Quartz
- QCPlugInInputImageSource
-  unbindTextureRepresentation(fromCGLContext:textureUnit:) Deprecated

Instance Method

# unbindTextureRepresentation(fromCGLContext:textureUnit:)

Unbinds the texture from a texture unit.

macOS 10.5–10.14Deprecated

``` source
func unbindTextureRepresentation(
    fromCGLContext cgl_ctx: CGLContextObj!,
    textureUnit unit: GLenum
)
```

**Required**

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`cgl_ctx`  

A CGL context.)

`unit`  

The texture unit to unbind from (such as, `GL_TEXTURE0`)

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

func bindTextureRepresentation(toCGLContext: CGLContextObj!, textureUnit: GLenum, normalizeCoordinates: Bool)

Binds the texture to a given texture unit and optionally scales or flips the texture.

**Required**

Deprecated

func unlockBufferRepresentation()

Releases the memory buffer representation of the image source.

**Required**

Deprecated

