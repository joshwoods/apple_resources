

- Compression
-  COMPRESSION_BROTLI 

Global Variable

# COMPRESSION_BROTLI

The Brotli compression algorithm, which is recommended for text compression.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var COMPRESSION_BROTLI: compression_algorithm { get }
```

## Discussion

The Brotli compression algorithm is a widely adopted content encoding method for the web. The Compression framework includes Brotli to provide decoding capabilities.

The Compression framework implements the Brotli level 2 encoder only. This compression level provides a good balance between compression speed and compression ratio. The Brotli decoder supports decoding data compressed with any compression level.

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

var COMPRESSION_LZBITMAP: compression_algorithm

The LZBITMAP compression algorithm, which is designed to exploit the vector instruction set of current CPUs.

