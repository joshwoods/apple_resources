

- Compression
-  compression_stream_init(\_:\_:\_:) 

Function

# compression_stream_init(\_:\_:\_:)

Initializes a compression stream for either compression or decompression.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func compression_stream_init(
    _ stream: UnsafeMutablePointer,
    _ operation: compression_stream_operation,
    _ algorithm: compression_algorithm
) -> compression_status
```

## Parameters 

`stream`  

Pointer to an allocated compression_stream structure.

`operation`  

A constant of type compression_stream_operation used to indicate the stream operation.

`algorithm`  

A constant of type compression_algorithm to select the algorithm: COMPRESSION_LZ4, COMPRESSION_ZLIB, COMPRESSION_LZMA, or COMPRESSION_LZFSE.

### Return Value

A value of type compression_status, interpreted as follows:

- COMPRESSION_STATUS_OK means the stream object was successfully initialized.

- COMPRESSION_STATUS_ERROR means an error occurred.

## Discussion

After success of this function, set the `dst_ptr`, `dst_size`, `src_ptr`, and `src_size` fields of the stream structure to their respective values. You can then pass stream structure to the compression_stream_process(_:_:) function.

## See Also

### Multiple-step compression

struct compression_stream

A structure representing a compression stream.

func compression_stream_process(UnsafeMutablePointer&lt;compression_stream>, Int32) -> compression_status

Performs compression or decompression using an initialized compression stream structure.

func compression_stream_destroy(UnsafeMutablePointer&lt;compression_stream>) -> compression_status

Frees any memory allocated by stream initialization function.

struct compression_status

A set of values used to represent the status of stream compression.

struct compression_stream_flags

A set of values used to represent stream compression flags.

struct compression_stream_operation

A set of values used to represent a stream compression operation.

struct compression_algorithm

A structure for values that represent compression algorithms.

