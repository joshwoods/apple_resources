

- Quartz
- QCPlugInInputImageSource
-  textureTarget() Deprecated

Instance Method

# textureTarget()

Returns the texture target.

macOS 10.5–10.14Deprecated

``` source
func textureTarget() -> GLenum
```

**Required**

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Return Value

The texture target, either `GL_TEXTURE_2D` or `GL_TEXTURE_RECTANGLE_EXT`.

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

func textureMatrix() -> UnsafePointer&lt;GLfloat>!

Returns a texture matrix.

**Required**

Deprecated

