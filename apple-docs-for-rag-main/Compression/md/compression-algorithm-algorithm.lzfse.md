

- Compression
- Algorithm
-  Algorithm.lzfse 

Case

# Algorithm.lzfse

The LZFSE compression algorithm, which is recommended for use on Apple platforms.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
case lzfse
```

## Discussion

LZFSE is Apple’s proprietary compression algorithm, matching the compression ratio of zlib level 5, but with much higher energy efficiency and speed (between 2x and 3x) for both encode and decode operations.

Use LZFSE when compressing a payload for iOS, macOS, watchOS, and tvOS. If you need to compress a payload for another platform (for example, Linux or Windows), use LZ4, LZMA, or zlib.

## See Also

### Related Documentation

var COMPRESSION_LZFSE: compression_algorithm

The LZFSE compression algorithm, which is recommended for use on Apple platforms.

