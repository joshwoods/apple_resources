

- FSKit
- FSMetadataRange
-  init(offset:segmentLength:segmentCount:) 

Initializer

# init(offset:segmentLength:segmentCount:)

Initializes a metadata range with the given properties.

macOS 15.4+

``` source
init(
    offset startOffset: off_t,
    segmentLength: UInt64,
    segmentCount: UInt64
)
```

## Parameters 

`startOffset`  

The start offset of the range in bytes. Ensure this value is a multiple of the corresponding resource’s blockSize.

`segmentLength`  

The segment length in bytes. Ensure this value is a multiple of the corresponding resource’s blockSize.

`segmentCount`  

The number of segments in the range.

