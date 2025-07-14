

- Metal
- MTLDevice
-  counterSets 

Instance Property

# counterSets

The counter sets supported by the device object.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var counterSets: [any MTLCounterSet]? { get }
```

**Required**

## Mentioned in 

Confirming which Counters and Counter Sets a GPU Supports

## See Also

### Sampling a GPU Device’s Counters

func supportsCounterSampling(MTLCounterSamplingPoint) -> Bool

Returns a Boolean value that indicates whether you can read GPU counters at the specified command boundary.

**Required**

enum MTLCounterSamplingPoint

Options for different times when you can sample GPU counters.

func makeCounterSampleBuffer(descriptor: MTLCounterSampleBufferDescriptor) throws -> any MTLCounterSampleBuffer

Creates a counter sample buffer.

**Required**

