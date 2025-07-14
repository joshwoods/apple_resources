

- Metal
- MTLCounterSampleBufferDescriptor
-  label 

Instance Property

# label

The name for the counter sample buffer you create with the descriptor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var label: String { get set }
```

## See Also

### Configuring a Descriptor for a Counter Sample Buffer

var counterSet: (any MTLCounterSet)?

A GPU device’s counter set instance that you want to sample.

var sampleCount: Int

The number of instances of a counter set’s data that a counter sample buffer can store.

var storageMode: MTLStorageMode

The memory storage mode for the counter sample buffers you create with the descriptor.

