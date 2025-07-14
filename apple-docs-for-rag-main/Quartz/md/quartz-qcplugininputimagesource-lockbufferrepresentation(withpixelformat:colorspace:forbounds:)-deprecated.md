

- Quartz
- QCPlugInInputImageSource
-  lockBufferRepresentation(withPixelFormat:colorSpace:forBounds:) Deprecated

Instance Method

# lockBufferRepresentation(withPixelFormat:colorSpace:forBounds:)

Creates a memory buffer representation from a subregion of the image source using the provided pixel format and color space.

macOS 10.4–10.15Deprecated

``` source
func lockBufferRepresentation(
    withPixelFormat format: String!,
    colorSpace: CGColorSpace!,
    forBounds bounds: NSRect
) -> Bool
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`format`  

A pixel format that is compatible with the color space.

`colorSpace`  

A Quartz color space that is compatible with the pixel format.

`bounds`  

The bounds of the subregion, expressed as pixels, and aligned to integer boundaries.

## Return Value

true if successful; otherwise false.

## Discussion

The content of the buffer is read-only. You should not attempt to modify it.

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

