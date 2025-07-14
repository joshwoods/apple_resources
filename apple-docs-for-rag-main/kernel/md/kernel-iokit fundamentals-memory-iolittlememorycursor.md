

- Kernel
- IOKit Fundamentals
- Memory
-  IOLittleMemoryCursor 

Class

# IOLittleMemoryCursor

An IOMemoryCursor subclass that outputs a vector of PhysicalSegments in the little endian byte order.

macOS 10.0+

``` source
class IOLittleMemoryCursor : IOMemoryCursor
```

## Overview

The IOLittleMemoryCursor would be used when the DMA hardware requires a little endian address and length pair. This cursor outputs an array of PhysicalSegments that are encoded in little endian format.

## Topics

### Miscellaneous

getPhysicalSegments

Generates a little endian physical scatter/gather list given a memory descriptor.

initWithSpecification

Primary initializer for the IOLittleMemoryCursor class.

outputSegment

Outputs the given segment into the output segments array in little endian byte order.

withSpecification

Creates and initializes an IOLittleMemoryCursor in one operation.

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

IOBigMemoryCursor

An IOMemoryCursor subclass that outputs a vector of PhysicalSegments in the big endian byte order.

IONaturalMemoryCursor

An IOMemoryCursor subclass that outputs a vector of PhysicalSegments in the natural byte orientation for the CPU.

IOMemoryCursor

A mechanism to convert memory references to physical addresses.

