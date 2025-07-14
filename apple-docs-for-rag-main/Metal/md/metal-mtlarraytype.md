

- Metal
-  MTLArrayType 

Class

# MTLArrayType

A description of an array.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLArrayType
```

## Overview

A MTLArrayType object provides details about an array parameter. Don’t create MTLArrayType objects directly; other reflection objects contain properties to determine if a parameter is an array and to obtain the MTLArrayType object that describes the array.

## Topics

### Describing the Array Elements

var arrayLength: Int

The number of elements in the array.

var elementType: MTLDataType

The data type of the array’s elements.

var stride: Int

The stride between array elements, in bytes.

var argumentIndexStride: Int

The stride, in bytes, between argument indices.

### Obtaining Details for Complex Array Elements

func element() -> MTLArrayType?

Provides a description of the underlying type when an array holds other arrays as its elements.

func elementStructType() -> MTLStructType?

Provides a description of the underlying struct type when an array holds structs as its elements.

func elementPointerType() -> MTLPointerType?

Provides a description of the underlying pointer type when an array holds pointers as its elements.

func elementTextureReferenceType() -> MTLTextureReferenceType?

Provides a description of the underlying texture type when an array holds textures as its elements.

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

class MTLStructType

A description of a structure.

class MTLStructMember

An object that provides information about a field in a structure.

class MTLPointerType

A description of a pointer.

class MTLTextureReferenceType

A description of a texture.

