

- Metal
- MTLDevice
-  supportsCounterSampling(\_:) 

Instance Method

# supportsCounterSampling(\_:)

Returns a Boolean value that indicates whether you can read GPU counters at the specified command boundary.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func supportsCounterSampling(_ samplingPoint: MTLCounterSamplingPoint) -> Bool
```

**Required**

## Parameters 

`samplingPoint`  

The command boundary to test.

## Mentioned in 

Sampling GPU Data into Counter Sample Buffers

## See Also

### Sampling a GPU Device’s Counters

var counterSets: [any MTLCounterSet]?

The counter sets supported by the device object.

**Required**

enum MTLCounterSamplingPoint

Options for different times when you can sample GPU counters.

func makeCounterSampleBuffer(descriptor: MTLCounterSampleBufferDescriptor) throws -> any MTLCounterSampleBuffer

Creates a counter sample buffer.

**Required**

