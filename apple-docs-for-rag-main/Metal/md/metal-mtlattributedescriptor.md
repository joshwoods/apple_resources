

- Metal
-  MTLAttributeDescriptor 

Class

# MTLAttributeDescriptor

A descriptor of an argument’s format and where its data is in memory.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class MTLAttributeDescriptor
```

## Overview

Attribute descriptors are part of an MTLVertexDescriptor or MTLStageInputOutputDescriptor instance to provide layout information about a function’s arguments. Each descriptor is for a single argument, containing information about the attached data, offset and stride, and data type.

## Topics

### Defining Attribute Location

var bufferIndex: Int

The index in the buffer argument table for the buffer that contains the data for this attribute.

var offset: Int

The offset, in bytes, from the start of the buffer containing the attribute data to the start of the data itself.

var format: MTLAttributeFormat

The format of the attribute’s data.

enum MTLAttributeFormat

Values indicating the organization and format of data for function attributes.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Configuring Compute Pass Inputs

var stageInputDescriptor: MTLStageInputOutputDescriptor?

The organization of input and output data for the next kernel call.

class MTLAttributeDescriptorArray

An array of attribute descriptor objects.

class MTLBufferLayoutDescriptor

A description of how a compute function fetches input data for an attribute.

class MTLBufferLayoutDescriptorArray

An array of buffer layout descriptor objects.

