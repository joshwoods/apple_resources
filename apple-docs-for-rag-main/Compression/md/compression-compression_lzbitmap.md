

- Compression
-  COMPRESSION_LZBITMAP 

Global Variable

# COMPRESSION_LZBITMAP

The LZBITMAP compression algorithm, which is designed to exploit the vector instruction set of current CPUs.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var COMPRESSION_LZBITMAP: compression_algorithm { get }
```

## Discussion

The LZBITMAP compression algorithm provides compression ratios as close as possible to COMPRESSION_ZLIB and COMPRESSION_LZFSE, with a lower compression cost. This compression algorithm is available only for the Compression buffer API functions, compression_encode_buffer(_:_:_:_:_:_:) and compression_decode_buffer(_:_:_:_:_:_:).

COMPRESSION_LZBITMAP is available only on Apple devices.

## See Also

### Algorithm Constants

var COMPRESSION_LZFSE: compression_algorithm

The LZFSE compression algorithm, which is recommended for use on Apple platforms.

var COMPRESSION_LZ4: compression_algorithm

The LZ4 compression algorithm for fast compression.

var COMPRESSION_LZ4_RAW: compression_algorithm

The LZ4 compression algorithm, without frame headers.

var COMPRESSION_LZMA: compression_algorithm

The LZMA compression algorithm, which is recommended for high-compression ratio.

var COMPRESSION_ZLIB: compression_algorithm

The zlib compression algorithm, which is recommended for cross-platform compression.

var COMPRESSION_BROTLI: compression_algorithm

The Brotli compression algorithm, which is recommended for text compression.

