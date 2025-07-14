

- Metal
-  MTLBinding 

Protocol

# MTLBinding

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol MTLBinding : NSObjectProtocol
```

## Topics

### Instance Properties

var access: MTLBindingAccess

**Required**

var index: Int

**Required**

var isArgument: Bool

**Required**

var isUsed: Bool

**Required**

var name: String

**Required**

var type: MTLBindingType

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- MTLBufferBinding
- MTLObjectPayloadBinding
- MTLTextureBinding
- MTLThreadgroupBinding

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

enum MTLBindingAccess

protocol MTLBufferBinding

protocol MTLTextureBinding

protocol MTLThreadgroupBinding

protocol MTLObjectPayloadBinding

