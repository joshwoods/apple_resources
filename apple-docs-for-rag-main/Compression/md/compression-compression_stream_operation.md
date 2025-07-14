

- Compression
-  compression_stream_operation 

Structure

# compression_stream_operation

A set of values used to represent a stream compression operation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct compression_stream_operation
```

## Topics

### Operation Constants

var COMPRESSION_STREAM_ENCODE: compression_stream_operation

A constant indicating a compression operation.

var COMPRESSION_STREAM_DECODE: compression_stream_operation

A constant indicating a decompression operation.

### Initializers

init(UInt32)

Creates a new constant from the given raw value.

init(rawValue: UInt32)

Creates a new constant from the given raw value.

### Instance Properties

var rawValue: UInt32

The raw value of the constant.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Multiple-step compression

struct compression_stream

A structure representing a compression stream.

func compression_stream_init(UnsafeMutablePointer&lt;compression_stream>, compression_stream_operation, compression_algorithm) -> compression_status

Initializes a compression stream for either compression or decompression.

func compression_stream_process(UnsafeMutablePointer&lt;compression_stream>, Int32) -> compression_status

Performs compression or decompression using an initialized compression stream structure.

func compression_stream_destroy(UnsafeMutablePointer&lt;compression_stream>) -> compression_status

Frees any memory allocated by stream initialization function.

struct compression_status

A set of values used to represent the status of stream compression.

struct compression_stream_flags

A set of values used to represent stream compression flags.

struct compression_algorithm

A structure for values that represent compression algorithms.

