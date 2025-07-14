

- Metal
-  MTLBufferLayoutDescriptor 

Class

# MTLBufferLayoutDescriptor

A description of how a compute function fetches input data for an attribute.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class MTLBufferLayoutDescriptor
```

## Topics

### Describing Fetch Behavior

var stride: Int

The number of bytes from one buffer entry to the next.

var stepFunction: MTLStepFunction

Determines how and when compute functions fetch data.

var stepRate: Int

How frequently the step function should load data.

enum MTLStepFunction

The frequency and locations at which a function fetches attribute data.

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

class MTLAttributeDescriptor

A descriptor of an argument’s format and where its data is in memory.

class MTLAttributeDescriptorArray

An array of attribute descriptor objects.

class MTLBufferLayoutDescriptorArray

An array of buffer layout descriptor objects.

