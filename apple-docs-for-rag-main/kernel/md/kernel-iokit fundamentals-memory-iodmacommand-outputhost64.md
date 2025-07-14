

- Kernel
- IOKit Fundamentals
- Memory
- IODMACommand
-  OutputHost64 

# OutputHost64

Output host natural Segment64 output segment function.

``` source
static bool OutputHost64(
 IODMACommand *target, 
 Segment64 seg,
 void *segs,
 UInt32 ind); 
```

## See Also

### Managing Memory Segments

Segment32

A 32 bit I/O bus address/length pair.

Segment64

A 64 bit I/O bus address/length pair.

SegmentFunction

A C function that translates a 64-bit segment and outputs a single desired segment to the specified array.

kIODMACommandOutputBig32

Output big-endian Segment32 output segment function.

OutputBig32

Output big-endian Segment32 output segment function.

+ OutputBig32

Output big-endian Segment32 output segment function.

kIODMACommandOutputBig64

Output big-endian Segment64 output segment function.

OutputBig64

Output big-endian Segment64 output segment function.

+ OutputBig64

Output big-endian Segment64 output segment function.

kIODMACommandOutputHost32

Output host natural Segment32 output segment function.

OutputHost32

Output host natural Segment32 output segment function.

+ OutputHost32

Output host natural Segment32 output segment function.

kIODMACommandOutputHost64

Output host natural Segment64 output segment function.

+ OutputHost64

Output host natural Segment64 output segment function.

kIODMACommandOutputLittle32

Output little-endian Segment32 output segment function.

OutputLittle32

Output little-endian Segment32 output segment function.

+ OutputLittle32

Output little-endian Segment32 output segment function.

kIODMACommandOutputLittle64

Output little-endian Segment64 output segment function.

OutputLittle64

Output little-endian Segment64 output segment function.

+ OutputLittle64

Output little-endian Segment64 output segment function.

