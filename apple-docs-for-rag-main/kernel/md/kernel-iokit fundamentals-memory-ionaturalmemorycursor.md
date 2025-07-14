

- Kernel
- IOKit Fundamentals
- Memory
-  IONaturalMemoryCursor 

Class

# IONaturalMemoryCursor

An IOMemoryCursor subclass that outputs a vector of PhysicalSegments in the natural byte orientation for the CPU.

macOS 10.0+

``` source
class IONaturalMemoryCursor : IOMemoryCursor
```

## Overview

The IONaturalMemoryCursor would be used when it is too difficult to safely describe a SegmentFunction that is more appropriate for your hardware. This cursor just outputs an array of PhysicalSegments.

## Topics

### Miscellaneous

getPhysicalSegments

Generates a CPU natural physical scatter/gather list given a memory descriptor.

initWithSpecification

Primary initializer for the IONaturalMemoryCursor class.

outputSegment

Outputs the given segment into the output segments array in natural byte order.

withSpecification

Creates and initializes an IONaturalMemoryCursor in one operation.

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

IOLittleMemoryCursor

An IOMemoryCursor subclass that outputs a vector of PhysicalSegments in the little endian byte order.

IOMemoryCursor

A mechanism to convert memory references to physical addresses.

