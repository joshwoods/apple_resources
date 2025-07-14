

- Metal
-  MTLTextureBinding 

Protocol

# MTLTextureBinding

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol MTLTextureBinding : MTLBinding
```

## Topics

### Instance Properties

var arrayLength: Int

**Required**

var isDepthTexture: Bool

**Required**

var textureDataType: MTLDataType

**Required**

var textureType: MTLTextureType

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

protocol MTLBufferBinding

protocol MTLThreadgroupBinding

protocol MTLObjectPayloadBinding

