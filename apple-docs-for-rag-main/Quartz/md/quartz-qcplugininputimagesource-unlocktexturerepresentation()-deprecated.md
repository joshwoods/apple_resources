

- Quartz
- QCPlugInInputImageSource
-  unlockTextureRepresentation() Deprecated

Instance Method

# unlockTextureRepresentation()

Releases the OpenGL texture representation of the image source.

macOS 10.5–10.14Deprecated

``` source
func unlockTextureRepresentation()
```

**Required**

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## See Also

### Converting an Image to a Representation

func lockTextureRepresentation(with: CGColorSpace!, forBounds: NSRect) -> Bool

Creates an OpenGL texture representation from a subregion of the image source using the provided color space.

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

func unbindTextureRepresentation(fromCGLContext: CGLContextObj!, textureUnit: GLenum)

Unbinds the texture from a texture unit.

**Required**

Deprecated

func unlockBufferRepresentation()

Releases the memory buffer representation of the image source.

**Required**

Deprecated

