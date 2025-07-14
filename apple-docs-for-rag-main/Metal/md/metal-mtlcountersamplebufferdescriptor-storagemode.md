

- Metal
- MTLCounterSampleBufferDescriptor
-  storageMode 

Instance Property

# storageMode

The memory storage mode for the counter sample buffers you create with the descriptor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var storageMode: MTLStorageMode { get set }
```

## Mentioned in 

Converting a GPU’s Counter Data into a Readable Format

Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass

## Discussion

To access a counter sample buffer with the CPU, set this property to MTLStorageMode.shared, otherwise MTLStorageMode.private.

## See Also

### Configuring a Descriptor for a Counter Sample Buffer

var counterSet: (any MTLCounterSet)?

A GPU device’s counter set instance that you want to sample.

var label: String

The name for the counter sample buffer you create with the descriptor.

var sampleCount: Int

The number of instances of a counter set’s data that a counter sample buffer can store.

