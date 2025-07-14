

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryCursor
-  SegmentFunction 

# SegmentFunction

A C function that translates a 64-bit segment and outputs a single desired segment to the specified array.

``` source
typedef bool ( *SegmentFunction)(
   IODMACommand *target,
   Segment64 segment,
   void *segments,
   UInt32 segmentIndex);
```

## Parameters 

`segment`  

The 64Bit I/O bus address and length.

`segments`  

Base of the output vector of DMA address length pairs.

`segmentIndex`  

Index to output 'segment' in the 'segments' array.

## Return Value

Returns true if segment encoding succeeded. false may be returned if the current segment does not fit in an output segment, i.e. a 38bit address wont fit into a 32 encoding.

## Overview

There are a group of pre-implemented SegmentFunctions that may be usefull to the developer below.

