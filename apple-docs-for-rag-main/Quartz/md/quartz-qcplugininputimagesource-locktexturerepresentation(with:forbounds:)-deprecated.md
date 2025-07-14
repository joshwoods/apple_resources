

- Quartz
- QCPlugInInputImageSource
-  lockTextureRepresentation(with:forBounds:) Deprecated

Instance Method

# lockTextureRepresentation(with:forBounds:)

Creates an OpenGL texture representation from a subregion of the image source using the provided color space.

macOS 10.5–10.14Deprecated

``` source
func lockTextureRepresentation(
    with colorSpace: CGColorSpace!,
    forBounds bounds: NSRect
) -> Bool
```

**Required**

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`colorSpace`  

A Quartz color space.

`bounds`  

The bounds of the subregion, expressed in pixels. They must be aligned to integer boundaries.

## Return Value

true is successful; false if texture can’t be created.

## Discussion

Neither the content of the texture nor its states (for example, the wrap mode) must be modified; you can only draw with it. The texture is valid only in the plug-in context.

## See Also

### Converting an Image to a Representation

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

func unlockBufferRepresentation()

Releases the memory buffer representation of the image source.

**Required**

Deprecated

