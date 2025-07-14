

- Metal
-  MTLBufferBinding 

Protocol

# MTLBufferBinding

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol MTLBufferBinding : MTLBinding
```

## Topics

### Instance Properties

var bufferAlignment: Int

**Required**

var bufferDataSize: Int

**Required**

var bufferDataType: MTLDataType

**Required**

var bufferPointerType: MTLPointerType?

**Required**

var bufferStructType: MTLStructType?

**Required**

## Relationships

### Inherits From

- MTLBinding
- NSObjectProtocol

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

enum MTLBindingType

protocol MTLBinding

enum MTLBindingAccess

protocol MTLTextureBinding

protocol MTLThreadgroupBinding

protocol MTLObjectPayloadBinding

