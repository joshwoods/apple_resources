

- Metal Performance Shaders
-  MPSCommandBuffer 

Class

# MPSCommandBuffer

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
class MPSCommandBuffer : NSObject
```

## Topics

### Initializers

init(commandBuffer: any MTLCommandBuffer)

init(from: any MTLCommandQueue)

### Instance Properties

var commandBuffer: any MTLCommandBuffer

var heapProvider: (any MPSHeapProvider)?

var predicate: MPSPredicate?

var rootCommandBuffer: any MTLCommandBuffer

### Instance Methods

func commitAndContinue()

func prefetchHeap(forWorkloadSize: Int)

## Relationships

### Inherits From

- NSObject

### Conforms To

- MTLCommandBuffer

