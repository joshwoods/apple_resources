

- Metal
-  MTLTextureReferenceType 

Class

# MTLTextureReferenceType

A description of a texture.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MTLTextureReferenceType
```

## Topics

### Describing the Texture

var textureType: MTLTextureType

The texture type of the texture.

var textureDataType: MTLDataType

The data type of the texture.

var access: MTLBindingAccess

The texture’s read/write access to the argument.

var isDepthTexture: Bool

A Boolean value that indicates whether the texture is a depth texture.

## Relationships

### Inherits From

- MTLType

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Shader Types

class MTLType

A description of a data type.

enum MTLDataType

The types of GPU functions, including shaders and compute kernels.

class MTLArrayType

A description of an array.

class MTLStructType

A description of a structure.

class MTLStructMember

An object that provides information about a field in a structure.

class MTLPointerType

A description of a pointer.

