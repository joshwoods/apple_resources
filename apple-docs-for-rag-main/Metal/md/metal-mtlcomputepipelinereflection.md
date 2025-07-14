

- Metal
-  MTLComputePipelineReflection 

Class

# MTLComputePipelineReflection

Information about the arguments of a compute function.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
class MTLComputePipelineReflection
```

## Overview

An MTLComputePipelineReflection object provides access to the arguments of the compute function used in an MTLComputePipelineState object. An MTLComputePipelineReflection object can be created along with an MTLComputePipelineState object. Don’t create an MTLComputePipelineReflection object directly. Instead, call either the makeComputePipelineState(function:options:reflection:) or makeComputePipelineState(function:options:completionHandler:) method of MTLDevice to create both an MTLComputePipelineState object and an MTLComputePipelineReflection object.

MTLComputePipelineReflection objects can use a significant amount of memory; release any strong references to them after you finish creating pipeline objects.

## Topics

### Obtaining the Arguments of the Compute Function

var arguments: [MTLArgument]

An array of objects that describe the arguments of a compute function.

Deprecated

### Instance Properties

var bindings: [any MTLBinding]

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

### Introspection Data

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

protocol MTLTextureBinding

protocol MTLThreadgroupBinding

protocol MTLObjectPayloadBinding

