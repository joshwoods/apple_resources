

- Metal
-  MTLAttribute 

Class

# MTLAttribute

An object that describes an attribute defined in the stage-in argument for a shader.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class MTLAttribute
```

## Topics

### Reading an Attribute’s Properties

var name: String

The name of the attribute.

var attributeIndex: Int

The index of the attribute, as declared in Metal shader source code.

var attributeType: MTLDataType

The data type for the attribute, as declared in Metal shader source code.

var isActive: Bool

A Boolean value that indicates whether the attribute is active.

var isPatchControlPointData: Bool

A Boolean value that indicates whether the attribute represents control point data.

var isPatchData: Bool

A Boolean value that indicates whether the attribute represents tessellation patch data.

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

class MTLVertexAttribute

An object that represents an attribute of a vertex function.

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

