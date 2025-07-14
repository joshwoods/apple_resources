

- Metal
-  MTLBindingType 

Enumeration

# MTLBindingType

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum MTLBindingType
```

## Topics

### Enumeration Cases

case buffer

case imageblock

case imageblockData

case instanceAccelerationStructure

case intersectionFunctionTable

case objectPayload

case primitiveAccelerationStructure

case sampler

case texture

case threadgroupMemory

case visibleFunctionTable

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Introspection Data

class MTLComputePipelineReflection

Information about the arguments of a compute function.

typealias MTLAutoreleasedComputePipelineReflection

A convenience type alias for an autoreleased compute pipeline reflection object.

class MTLRenderPipelineReflection

Information about the arguments of a graphics function.

typealias MTLAutoreleasedRenderPipelineReflection

A convenience type alias for an autoreleased pipeline reflection instance.

protocol MTLBinding

enum MTLBindingAccess

protocol MTLBufferBinding

protocol MTLTextureBinding

protocol MTLThreadgroupBinding

protocol MTLObjectPayloadBinding

