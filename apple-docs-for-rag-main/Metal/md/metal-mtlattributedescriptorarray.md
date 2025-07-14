

- Metal
-  MTLAttributeDescriptorArray 

Class

# MTLAttributeDescriptorArray

An array of attribute descriptor objects.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class MTLAttributeDescriptorArray
```

## Overview

An MTLAttributeDescriptorArray defines the data format and index binding for the attribute argument table, using MTLAttributeDescriptor instances.

## Topics

### Accessing Attribute State Objects

subscript(Int) -> MTLAttributeDescriptor!

Returns the state of the specified attribute.

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

class MTLBufferLayoutDescriptor

A description of how a compute function fetches input data for an attribute.

class MTLBufferLayoutDescriptorArray

An array of buffer layout descriptor objects.

