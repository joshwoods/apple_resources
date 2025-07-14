

- Kernel
- IOKit Fundamentals
- Memory
-  IOMemoryCursor 

Class

# IOMemoryCursor

A mechanism to convert memory references to physical addresses.

macOS 10.0+

``` source
class IOMemoryCursor : OSObject
```

## Overview

The IOMemoryCursor declares the super class that all specific memory cursors must inherit from, but a memory cursor can be created without a specific format subclass by just providing a segment function to the initializers. This class does the difficult stuff of dividing a memory descriptor into a physical scatter/gather list appropriate for the target hardware.

A driver is expected to create a memory cursor and configure it to the limitations of its DMA hardware; for instance the memory cursor used by the FireWire SBP-2 protocol has a maximum physical segment size of 2^16 - 1 but the actual transfer size is unlimited. Thus it would create a cursor with a maxSegmentSize of 65535 and a maxTransfer size of UINT_MAX. It would also provide a SegmentFunction that can output a pagelist entry.

Below is the simplest example of a SegmentFunction:

void IONaturalMemoryCursor::outputSegment(PhysicalSegment segment,

void \* outSegments,

UInt32 outSegmentIndex)

{

((PhysicalSegment \*) outSegments)\[outSegmentIndex\] = segment;

}

## Topics

### Miscellaneous

genPhysicalSegments

Generates a physical scatter/gather list given a memory descriptor.

initWithSpecification

Primary initializer for the IOMemoryCursor class.

withSpecification

Creates and initializes an IOMemoryCursor in one operation.

### Callbacks

SegmentFunction

A C function that translates a 64-bit segment and outputs a single desired segment to the specified array.

### Constants

Miscellaneous Defines

### DataTypes

PhysicalSegment

### Instance Variables

outSeg

maxTransferSize

maxSegmentSize

alignMask

### Instance Methods

- genPhysicalSegments

- getMetaClass

- initWithSpecification

### Type Methods

+ withSpecification

## Relationships

### Inherits From

- OSObject

## See Also

### Cursors

IOBigMemoryCursor

An IOMemoryCursor subclass that outputs a vector of PhysicalSegments in the big endian byte order.

IOLittleMemoryCursor

An IOMemoryCursor subclass that outputs a vector of PhysicalSegments in the little endian byte order.

IONaturalMemoryCursor

An IOMemoryCursor subclass that outputs a vector of PhysicalSegments in the natural byte orientation for the CPU.

