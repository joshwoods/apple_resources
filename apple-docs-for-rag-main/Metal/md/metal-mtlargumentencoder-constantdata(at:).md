

- Metal
- MTLArgumentEncoder
-  constantData(at:) 

Instance Method

# constantData(at:)

Returns a pointer to an inline, constant-data argument within the argument buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func constantData(at index: Int) -> UnsafeMutableRawPointer
```

**Required**

## Parameters 

`index`  

The index of an inline, constant-data argument within the argument buffer. The value corresponds to either the index ID of a declaration in Metal Shading Language (MSL) or the index property of an MTLArgumentDescriptor instance.

## Return Value

A pointer to the location in the buffer to which you should write the constant data.

## Discussion

Constants declared contiguously in the Metal shading language (in an array or structure) are contiguous in memory. You can encode contiguous ranges of inlined constant data through a pointer to the first constant.

To encode inlined constant data into the argument buffer, perform a memory copy operation from your data’s source pointer to the returned destination pointer.

- Swift
- Objective-C

```
let sourceConstants: [SourceConstants] = [
    // Inlined constant data.
    /* ... */
]
let destinationPointer = abEncoder.constantData(: 0)
destinationPointer.copyBytes(from: sourceConstants, count: MemoryLayout.size)
```

```
static const SourceConstants sourceConstants[] =
{    
    // Inlined constant data.
    /* ... */
};
void *destinationPointer = [abEncoder constantDataAtIndex:0];
memcpy(destinationPointer, sourceConstants, sizeof(SourceConstants));
```

