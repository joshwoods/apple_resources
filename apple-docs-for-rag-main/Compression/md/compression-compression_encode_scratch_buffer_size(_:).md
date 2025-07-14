

- Compression
-  compression_encode_scratch_buffer_size(\_:) 

Function

# compression_encode_scratch_buffer_size(\_:)

Returns the required compression scratch buffer size for the selected algorithm.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func compression_encode_scratch_buffer_size(_ algorithm: compression_algorithm) -> Int
```

## Parameters 

`algorithm`  

Set to the desired algorithm: COMPRESSION_LZ4, COMPRESSION_ZLIB, COMPRESSION_LZMA, or COMPRESSION_LZFSE.

## Return Value

Size in bytes.

## Discussion

This function returns the number of bytes to provide in an optional scratch buffer when calling compression_encode_buffer(_:_:_:_:_:_:).

## See Also

### Single-step compression

Compressing and decompressing data with buffer compression

Compress a string, write it to the file system, and decompress the same file using buffer compression.

func compression_encode_buffer(UnsafeMutablePointer&lt;UInt8>, Int, UnsafePointer&lt;UInt8>, Int, UnsafeMutableRawPointer?, compression_algorithm) -> Int

Compresses the contents of a source buffer into a destination buffer.

func compression_decode_scratch_buffer_size(compression_algorithm) -> Int

Returns the required decompression scratch buffer size for the selected algorithm.

func compression_decode_buffer(UnsafeMutablePointer&lt;UInt8>, Int, UnsafePointer&lt;UInt8>, Int, UnsafeMutableRawPointer?, compression_algorithm) -> Int

Decompresses the contents of a source buffer into a destination buffer.

struct compression_algorithm

A structure for values that represent compression algorithms.

