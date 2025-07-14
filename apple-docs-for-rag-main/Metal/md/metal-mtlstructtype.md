

- Metal
-  MTLStructType 

Class

# MTLStructType

A description of a structure.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLStructType
```

## Overview

MTLStructType is part of the reflection API that allows Metal framework code to query details of a struct that is passed as an argument of a Metal shading language function. Don’t create MTLStructType objects directly; instead query the bufferStructType property of a MTLArgument object, or call the structType() method for a MTLStructMember object. To examine the details of the struct, you can recursively drill down the members property of the MTLStructType object, which contains details about struct members, each of which is represented by a MTLStructMember object.

## Topics

### Obtaining Information about Struct Members

var members: [MTLStructMember]

An array of objects that describe the fields in the struct.

func memberByName(String) -> MTLStructMember?

Provides a representation of a struct member.

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

class MTLStructMember

An object that provides information about a field in a structure.

class MTLPointerType

A description of a pointer.

class MTLTextureReferenceType

A description of a texture.

