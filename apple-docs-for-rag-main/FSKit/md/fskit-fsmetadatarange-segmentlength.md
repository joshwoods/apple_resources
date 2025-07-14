

- FSKit
- FSMetadataRange
-  segmentLength 

Instance Property

# segmentLength

The segment length in bytes.

macOS 15.4+

``` source
var segmentLength: UInt64 { get }
```

## Discussion

Ensure this value is a multiple of the corresponding resource’s blockSize.

## See Also

### Accessing range properties

var startOffset: off_t

The start offset of the range in bytes.

var segmentCount: UInt64

The number of segments in the range.

