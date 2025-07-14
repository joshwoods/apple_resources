

- Kernel
- IOKit Fundamentals
- Memory
-  IOBigMemoryCursor 

Class

# IOBigMemoryCursor

An IOMemoryCursor subclass that outputs a vector of PhysicalSegments in the big endian byte order.

macOS 10.0+

``` source
class IOBigMemoryCursor : IOMemoryCursor
```

## Overview

The IOBigMemoryCursor would be used when the DMA hardware requires a big endian address and length pair. This cursor outputs an array of PhysicalSegments that are encoded in big-endian format.

## Topics

### Miscellaneous

getPhysicalSegments

Generates a big endian physical scatter/gather list given a memory descriptor.

initWithSpecification

Primary initializer for the IOBigMemoryCursor class.

outputSegment

Outputs the given segment into the output segments array in big endian byte order.

withSpecification

Creates and initializes an IOBigMemoryCursor in one operation.

### Constants

Miscellaneous Defines

### Instance Methods

- getMetaClass

- getPhysicalSegments

- initWithSpecification

### Type Methods

+ outputSegment

+ withSpecification

## Relationships

### Inherits From

- IOMemoryCursor

## See Also

### Cursors

IOLittleMemoryCursor

An IOMemoryCursor subclass that outputs a vector of PhysicalSegments in the little endian byte order.

IONaturalMemoryCursor

An IOMemoryCursor subclass that outputs a vector of PhysicalSegments in the natural byte orientation for the CPU.

IOMemoryCursor

A mechanism to convert memory references to physical addresses.

