

- Quartz
- QCPlugInInputImageSource
-  unlockBufferRepresentation() Deprecated

Instance Method

# unlockBufferRepresentation()

Releases the memory buffer representation of the image source.

macOS 10.4–10.15Deprecated

``` source
func unlockBufferRepresentation()
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

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

func unbindTextureRepresentation(fromCGLContext: CGLContextObj!, textureUnit: GLenum)

Unbinds the texture from a texture unit.

**Required**

Deprecated

