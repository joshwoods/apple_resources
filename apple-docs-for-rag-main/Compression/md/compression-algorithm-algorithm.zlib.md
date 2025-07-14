

- Compression
- Algorithm
-  Algorithm.zlib 

Case

# Algorithm.zlib

The zlib compression algorithm, which is recommended for cross-platform compression.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
case zlib
```

## Discussion

The Compression library implements the zlib encoder at level 5 only. This compression level provides a good balance between compression speed and compression ratio. The zlib decoder supports decoding data compressed with any compression level.

The encoded format is the raw `DEFLATE` format as described in IETF RFC 1951, the following obtains the equivalent configuration of the encoder:

```
```

## See Also

### Related Documentation

var COMPRESSION_ZLIB: compression_algorithm

The zlib compression algorithm, which is recommended for cross-platform compression.

