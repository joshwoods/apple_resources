

- Metal
- MTLCounterSampleBufferDescriptor
-  sampleCount 

Instance Property

# sampleCount

The number of instances of a counter set’s data that a counter sample buffer can store.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var sampleCount: Int { get set }
```

## Mentioned in 

Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass

## Discussion

The counter sample buffer instances you create with the MTLCounterSampleBufferDescriptor can store sampleCount instances of a counter set.

## See Also

### Configuring a Descriptor for a Counter Sample Buffer

var counterSet: (any MTLCounterSet)?

A GPU device’s counter set instance that you want to sample.

var label: String

The name for the counter sample buffer you create with the descriptor.

var storageMode: MTLStorageMode

The memory storage mode for the counter sample buffers you create with the descriptor.

