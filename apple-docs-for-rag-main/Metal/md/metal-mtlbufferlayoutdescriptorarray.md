

- Metal
-  MTLBufferLayoutDescriptorArray 

Class

# MTLBufferLayoutDescriptorArray

An array of buffer layout descriptor objects.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class MTLBufferLayoutDescriptorArray
```

## Overview

An MTLBufferLayoutDescriptorArray defines the data layout and loading for compute data, using MTLBufferLayoutDescriptor instances.

## Topics

### Array Accessors

subscript(Int) -> MTLBufferLayoutDescriptor!

Returns the state of the specified buffer layout.

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

### Configuring Compute Pass Inputs

var stageInputDescriptor: MTLStageInputOutputDescriptor?

The organization of input and output data for the next kernel call.

class MTLAttributeDescriptor

A descriptor of an argument’s format and where its data is in memory.

class MTLAttributeDescriptorArray

An array of attribute descriptor objects.

class MTLBufferLayoutDescriptor

A description of how a compute function fetches input data for an attribute.

