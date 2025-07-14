

- Dispatch
-  DISPATCH_IO_STREAM 

Global Variable

# DISPATCH_IO_STREAM

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var DISPATCH_IO_STREAM: Int32 { get }
```

## Discussion

The channel represents a linear stream of bytes. Read and write operations are performed serially in the order they were started. Operations always read or write data at the file pointer position that is current when the read or write begins. Read and write operations may be performed simultaneously on the same channel.

Offset values are ignored for channels of this type.

## See Also

### Initializing the Type

var DISPATCH_IO_RANDOM: Int32

