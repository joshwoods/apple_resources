

- Metal
-  MTLCounterSampleBuffer 

Protocol

# MTLCounterSampleBuffer

A specialized memory buffer that stores a GPU’s counter set data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
protocol MTLCounterSampleBuffer : NSObjectProtocol
```

## Mentioned in 

Converting a GPU’s Counter Data into a Readable Format

Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass

Confirming which Counters and Counter Sets a GPU Supports

Sampling GPU Data into Counter Sample Buffers

Converting GPU Timestamps into CPU Time

## Overview

Create a counter sample buffer by calling an MTLDevice instance’s makeCounterSampleBuffer(descriptor:) method. See Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass.

You can store a GPU device’s counter set data only with an MTLCounterSampleBuffer instance that you create from the same device. See Sampling GPU Data into Counter Sample Buffers for information about storing counter sample data in a counter sample buffer.

## Topics

### Resolving the Counter Sample Buffer’s Data

func resolveCounterRange(Range&lt;Int>) throws -> Data?

Transforms samples of a GPU’s counter set from the driver’s internal format to a standard Metal data structure.

### Inspecting the Counter Sample Buffer’s Configuration

var label: String

A string that identifies the counter sample buffer.

**Required**

var device: any MTLDevice

The GPU device instance that owns the counter sample buffer.

**Required**

var sampleCount: Int

The number of samples in the buffer.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Counter Sample Buffers

Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass

Make a buffer that provides a place for a GPU to save its runtime performance metrics as it runs a pass.

class MTLCounterSampleBufferDescriptor

A group of properties that configures the counter sample buffers you create with it.

Sampling GPU Data into Counter Sample Buffers

Retrieve a GPU’s counter data at a time the GPU supports.

var MTLCounterDontSample: Int

A sentinel value that instructs an encoder to skip sampling a counter as the GPU runs the encoder’s pass.

