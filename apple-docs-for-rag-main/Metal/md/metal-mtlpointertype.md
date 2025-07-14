

- Metal
-  MTLPointerType 

Class

# MTLPointerType

A description of a pointer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MTLPointerType
```

## Topics

### Describing the Pointer Elements

var alignment: Int

The required byte alignment in memory for the element data.

var dataSize: Int

The size, in bytes, of the element data.

var elementType: MTLDataType

The data type of the element data.

var access: MTLBindingAccess

The function’s read/write access to the element data.

var elementIsArgumentBuffer: Bool

A Boolean value that indicates whether the element is an argument buffer.

### Obtaining Details for Complex Pointer Elements

func elementArrayType() -> MTLArrayType?

Provides a description of the underlying array when the pointer points to an array.

func elementStructType() -> MTLStructType?

Provides a description of the underlying struct when the pointer points to a struct.

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

class MTLTextureReferenceType

A description of a texture.

