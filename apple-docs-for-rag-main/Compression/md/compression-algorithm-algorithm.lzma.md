

- Compression
- Algorithm
-  Algorithm.lzma 

Case

# Algorithm.lzma

The LZMA compression algorithm, which is recommended for high-compression ratio.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
case lzma
```

## Discussion

The Compression library implements the LZMA encoder at level 6 only. This is the default compression level for open source LZMA, and provides excellent compression. The LZMA decoder supports decoding data compressed with any compression level.

## See Also

### Related Documentation

var COMPRESSION_LZMA: compression_algorithm

The LZMA compression algorithm, which is recommended for high-compression ratio.

