

- FSKit
- FSMetadataRange
-  startOffset 

Instance Property

# startOffset

The start offset of the range in bytes.

macOS 15.4+

``` source
var startOffset: off_t { get }
```

## Discussion

Ensure this value is a multiple of the corresponding resource’s blockSize.

## See Also

### Accessing range properties

var segmentLength: UInt64

The segment length in bytes.

var segmentCount: UInt64

The number of segments in the range.

