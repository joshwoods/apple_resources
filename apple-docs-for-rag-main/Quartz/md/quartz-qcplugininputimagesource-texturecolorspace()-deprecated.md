

- Quartz
- QCPlugInInputImageSource
-  textureColorSpace() Deprecated

Instance Method

# textureColorSpace()

Returns the color space of the texture representation.

macOS 10.5–10.14Deprecated

``` source
func textureColorSpace() -> Unmanaged!
```

**Required**

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Return Value

The color space of the texture.

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

func textureFlipped() -> Bool

Returns whether or not the contents of the texture are flipped vertically.

**Required**

Deprecated

func textureMatrix() -> UnsafePointer&lt;GLfloat>!

Returns a texture matrix.

**Required**

Deprecated

