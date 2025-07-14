

- Compression
- Algorithm
-  Algorithm.lzbitmap 

Case

# Algorithm.lzbitmap

The LZBITMAP compression algorithm, which is designed to exploit the vector instruction set of current CPUs.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
case lzbitmap
```

## Discussion

The LZBITMAP compression algorithm provides compression ratios as close as possible to COMPRESSION_ZLIB and COMPRESSION_LZFSE, with a lower compression cost. This compression algorithm is available only for the Compression buffer API functions, compression_encode_buffer(_:_:_:_:_:_:) and compression_decode_buffer(_:_:_:_:_:_:).

COMPRESSION_LZBITMAP is available only on Apple devices.

