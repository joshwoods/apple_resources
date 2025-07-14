

- Metal
- MTLDevice
-  makeCounterSampleBuffer(descriptor:) 

Instance Method

# makeCounterSampleBuffer(descriptor:)

Creates a counter sample buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func makeCounterSampleBuffer(descriptor: MTLCounterSampleBufferDescriptor) throws -> any MTLCounterSampleBuffer
```

**Required**

## Parameters 

`descriptor`  

An MTLCounterSampleBufferDescriptor instance.

## Return Value

A new MTLCounterSampleBuffer instance if the method completes successfully; otherwise Swift throws an error and Objective-C returns `nil`.

## Mentioned in 

Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass

## Discussion

The method may produce an error if the GPU driver has exhausted its underlying resources for counter sample buffers.

## See Also

### Sampling a GPU Device’s Counters

var counterSets: [any MTLCounterSet]?

The counter sets supported by the device object.

**Required**

func supportsCounterSampling(MTLCounterSamplingPoint) -> Bool

Returns a Boolean value that indicates whether you can read GPU counters at the specified command boundary.

**Required**

enum MTLCounterSamplingPoint

Options for different times when you can sample GPU counters.

