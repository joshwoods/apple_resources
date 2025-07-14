

- Quartz
- QCPlugInInputImageSource
-  texturePixelsWide() Deprecated

Instance Method

# texturePixelsWide()

Returns the width of the texture representation.

macOS 10.5–10.14Deprecated

``` source
func texturePixelsWide() -> Int
```

**Required**

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Return Value

The width of the texture, expressed in pixels.

## See Also

### Getting Texture Information

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

func textureMatrix() -> UnsafePointer&lt;GLfloat>!

Returns a texture matrix.

**Required**

Deprecated

