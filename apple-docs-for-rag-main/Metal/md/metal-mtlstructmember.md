

- Metal
-  MTLStructMember 

Class

# MTLStructMember

An object that provides information about a field in a structure.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLStructMember
```

## Overview

MTLStructMember is part of the reflection API that allows Metal framework code to query details about an argument of a Metal shading language function. A MTLStructMember object describes the data type of one field in a struct that is passed as a MTLFunction argument, which is represented by MTLArgument.

Don’t create MTLStructMember objects directly. You obtain a MTLStructMember object from either the members property or the memberByName(_:) method of a MTLStructType object. The dataType property of the MTLStructMember object tells you what kind of data is stored in the member. Recursively drill down every struct member until you reach a data type that is neither a struct nor an array.

## Topics

### Describing the Struct Member

var name: String

The name of the struct member.

var dataType: MTLDataType

The data type of the struct member.

var offset: Int

The location of this member relative to the start of its struct, in bytes.

var argumentIndex: Int

The index in the argument table that corresponds to the struct member.

### Obtaining Struct Member Details

func arrayType() -> MTLArrayType?

Provides a description of the underlying array when the struct member holds an array.

func structType() -> MTLStructType?

Provides a description of the underlying struct when the struct member holds a struct.

func pointerType() -> MTLPointerType?

Provides a description of the underlying pointer when the struct member holds a pointer.

func textureReferenceType() -> MTLTextureReferenceType?

Provides a description of the underlying texture when the struct member holds a texture.

## Relationships

### Inherits From

- NSObject

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

class MTLPointerType

A description of a pointer.

class MTLTextureReferenceType

A description of a texture.

