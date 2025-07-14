

- GLKit
-  GLKTextureInfo Deprecated

Class

# GLKTextureInfo

Information about OpenGL textures created by the GLKTextureLoader class.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedmacOS 10.8–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
class GLKTextureInfo
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Overview

When your app loads textures using the GLKTextureLoader class, the texture loader returns information about the textures using GLKTextureInfo objects. Your app never creates GLKTextureInfo objects directly.

## Topics

### Reading Texture Information

var name: GLuint

The OpenGL context’s name for the texture.

var target: GLenum

The OpenGL binding target for the texture.

var height: GLuint

The height of the loaded texture.

var width: GLuint

The width of the loaded texture.

var textureOrigin: GLKTextureInfoOrigin

The location of the origin in the loaded texture.

var alphaState: GLKTextureInfoAlphaState

The state of the alpha component in the loaded texture.

var containsMipmaps: Bool

A Boolean value that states whether the loaded texture contains mip maps.

### Constants

enum GLKTextureInfoAlphaState

Values that describe the alpha information stored in a source image’s pixel data.

enum GLKTextureInfoOrigin

The location of the origin in the original source image.

### Instance Properties

var arrayLength: GLuint

var depth: GLuint

var mimapLevelCount: GLuint

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Texture Loading

class GLKTextureLoader

A utility class that simplifies loading OpenGL or OpenGL ES texture datas from a variety of image file formats.

Deprecated

