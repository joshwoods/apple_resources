

- Kernel
- IOKit Fundamentals
- Memory
-  IODMAController 

Class

# IODMAController

macOS 10.5+

``` source
class IODMAController : IOService
```

## Topics

### Instance Methods

- completeDMACommand

- getFIFODepth

- getMetaClass

- initDMAChannel

- notifyDMACommand

- queryDMACommand

- registerDMAController

- setDMAConfig

- setFIFODepth

- setFrameSize

- start

- startDMACommand

- stopDMACommand

- validDMAConfig

- validFIFODepth

### Type Methods

+ createControllerName

+ getController

## Relationships

### Inherits From

- IOService

## See Also

### Direct Memory Access (DMA)

IODMACommand

An object that converts memory references to I/O bus addresses.

IODMAEventSource

