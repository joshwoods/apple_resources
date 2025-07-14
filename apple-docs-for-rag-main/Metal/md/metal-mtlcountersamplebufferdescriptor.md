

- Metal
-  MTLCounterSampleBufferDescriptor 

Class

# MTLCounterSampleBufferDescriptor

A group of properties that configures the counter sample buffers you create with it.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
class MTLCounterSampleBufferDescriptor
```

## Mentioned in 

Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass

## Overview

To create a new counter sample buffer, create and configure an MTLCounterSampleBufferDescriptor instance, and then call an MTLDevice instance’s makeCounterSampleBuffer(descriptor:) method. See Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass.

Each new sample counter buffer inherits the values of the descriptor’s properties when you create it. You can modify a descriptor and reuse it to create other counter sample buffers, which has no effect on existing counter sample buffers.

## Topics

### Configuring a Descriptor for a Counter Sample Buffer

var counterSet: (any MTLCounterSet)?

A GPU device’s counter set instance that you want to sample.

var label: String

The name for the counter sample buffer you create with the descriptor.

var sampleCount: Int

The number of instances of a counter set’s data that a counter sample buffer can store.

var storageMode: MTLStorageMode

The memory storage mode for the counter sample buffers you create with the descriptor.

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

### Counter Sample Buffers

Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass

Make a buffer that provides a place for a GPU to save its runtime performance metrics as it runs a pass.

protocol MTLCounterSampleBuffer

A specialized memory buffer that stores a GPU’s counter set data.

Sampling GPU Data into Counter Sample Buffers

Retrieve a GPU’s counter data at a time the GPU supports.

var MTLCounterDontSample: Int

A sentinel value that instructs an encoder to skip sampling a counter as the GPU runs the encoder’s pass.

