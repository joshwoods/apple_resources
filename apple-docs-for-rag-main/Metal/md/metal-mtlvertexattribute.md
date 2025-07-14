

- Metal
-  MTLVertexAttribute 

Class

# MTLVertexAttribute

An object that represents an attribute of a vertex function.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLVertexAttribute
```

## Overview

A MTLVertexAttribute object represents an attribute for per-vertex input in a vertex function. You use vertex attribute objects to inspect the inputs of a vertex function by examining the vertexAttributes property of the corresponding MTLFunction object.

## Topics

### Describing the Attribute

var name: String

The name of the attribute.

var attributeIndex: Int

The index of the attribute, as declared in Metal shader source code.

var attributeType: MTLDataType

The data type for the attribute, as declared in Metal shader source code.

var isActive: Bool

A Boolean value that indicates whether this vertex attribute is active.

var isPatchControlPointData: Bool

A Boolean value that indicates whether this vertex attribute represents control point data.

var isPatchData: Bool

A Boolean value that indicates whether this vertex attribute represents patch data.

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

### Function Arguments

class MTLAttribute

An object that describes an attribute defined in the stage-in argument for a shader.

class MTLArgument

Information about an argument of a graphics or compute function.

Deprecated

typealias MTLAutoreleasedArgument

A convenience type alias for an autoreleased argument instance.

Deprecated

enum MTLArgumentType

The resource type for an argument of a function.

Deprecated

typealias MTLArgumentAccess

Function access restrictions to argument data in the shading language code.

Deprecated

