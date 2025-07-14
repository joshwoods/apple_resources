

- GLKit
- GLKTextureInfo
-  name Deprecated

Instance Property

# name

The OpenGL context’s name for the texture.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
var name: GLuint { get }
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

Your app uses this identifier whenever it wants to bind the texture to a context.

## See Also

### Reading Texture Information

var target: GLenum

The OpenGL binding target for the texture.

Deprecated

var height: GLuint

The height of the loaded texture.

Deprecated

var width: GLuint

The width of the loaded texture.

Deprecated

var textureOrigin: GLKTextureInfoOrigin

The location of the origin in the loaded texture.

Deprecated

var alphaState: GLKTextureInfoAlphaState

The state of the alpha component in the loaded texture.

Deprecated

var containsMipmaps: Bool

A Boolean value that states whether the loaded texture contains mip maps.

Deprecated

