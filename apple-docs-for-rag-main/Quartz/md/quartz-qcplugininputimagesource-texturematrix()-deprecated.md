

- Quartz
- QCPlugInInputImageSource
-  textureMatrix() Deprecated

Instance Method

# textureMatrix()

Returns a texture matrix.

macOS 10.5–10.14Deprecated

``` source
func textureMatrix() -> UnsafePointer!
```

**Required**

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Return Value

A 4x4 texture matrix created by scaling (from \[`0`, pixels\] to \[`0`,`1`\]) and vertically flipping the texture coordinates; `NULL` if coordinate transformation is not required.

## Discussion

This method is provided as a convenience for 2D textures to take care of two issues:

- Coordinates for rectangular textures are expressed in pixels rather than the normalized units used for power-of-two textures. The coordinates need to be normalized before you can process the texture.

- Texture coordinates are typically flipped by OpenGL for processing on the GPU and need to be flipped to the original coordinates.

You can take care of these two issues simply by loading a the matrix returned by this method onto the OpenGL stack. If you are not sure that your texture needs either of these operations, you can load the matrix on the OpenGL stack anyway, as it acts as an identity matrix if it’s not needed.

## See Also

### Getting Texture Information

func texturePixelsWide() -> Int

Returns the width of the texture representation.

**Required**

Deprecated

func texturePixelsHigh() -> Int

Returns the height of the texture representation.

**Required**

Deprecated

func textureTarget() -> GLenum

Returns the texture target.

**Required**

Deprecated

func textureName() -> GLuint

Returns the texture name.

**Required**

Deprecated

func textureColorSpace() -> Unmanaged&lt;CGColorSpace>!

Returns the color space of the texture representation.

**Required**

Deprecated

func textureFlipped() -> Bool

Returns whether or not the contents of the texture are flipped vertically.

**Required**

Deprecated

