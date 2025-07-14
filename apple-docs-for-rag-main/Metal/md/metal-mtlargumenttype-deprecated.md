

- Metal
-  MTLArgumentType Deprecated

Enumeration

# MTLArgumentType

The resource type for an argument of a function.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
enum MTLArgumentType
```

## Topics

### Argument Types

case buffer

The argument is a buffer.

case threadgroupMemory

The argument is a pointer to threadgroup memory.

case texture

The argument is a texture.

case sampler

The argument is a texture sampler.

case imageblock

The argument is an imageblock.

case imageblockData

The argument is imageblock data.

case visibleFunctionTable

The argument is a visible function table.

case intersectionFunctionTable

The argument is an intersection function table.

case primitiveAccelerationStructure

The argument is a bottom-level ray tracing acceleraton structure for a set of primitives.

case instanceAccelerationStructure

The argument is a top-level ray tracing acceleration structure for a set of instances.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Function Arguments

class MTLAttribute

An object that describes an attribute defined in the stage-in argument for a shader.

class MTLVertexAttribute

An object that represents an attribute of a vertex function.

class MTLArgument

Information about an argument of a graphics or compute function.

Deprecated

typealias MTLAutoreleasedArgument

A convenience type alias for an autoreleased argument instance.

Deprecated

typealias MTLArgumentAccess

Function access restrictions to argument data in the shading language code.

Deprecated

