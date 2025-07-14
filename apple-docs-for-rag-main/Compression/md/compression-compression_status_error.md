

- Compression
-  COMPRESSION_STATUS_ERROR 

Global Variable

# COMPRESSION_STATUS_ERROR

Indicates an error with stream compression.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var COMPRESSION_STATUS_ERROR: compression_status { get }
```

## Discussion

If there’s an error with stream compression or decompression, for example if the encoded data is corrupted, compression_stream_process(_:_:) returns COMPRESSION_STATUS_ERROR.

## See Also

### Status Constants

var COMPRESSION_STATUS_OK: compression_status

Indicates the stream has consumed all data in the source buffer, or used all space in the destination buffer.

var COMPRESSION_STATUS_END: compression_status

Indicates the stream has read all input from the source, and written all output to the destination.

