

- Core Foundation
-  CFWriteStreamWrite(\_:\_:\_:) 

Function

# CFWriteStreamWrite(\_:\_:\_:)

Writes data to a writable stream.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFWriteStreamWrite(
    _ stream: CFWriteStream!,
    _ buffer: UnsafePointer!,
    _ bufferLength: CFIndex
) -> CFIndex
```

## Parameters 

`stream`  

The stream to which to write.

`buffer`  

The buffer holding the data to write.

`bufferLength`  

The number of bytes from `buffer` to write.

## Return Value

The number of bytes successfully written, `0` if the stream has been filled to capacity (for fixed-length streams), or `-1` if either the stream is not open or an error occurs.

## Discussion

If `stream` is in the process of opening, this function waits until it has completed. If the stream is not full, this call blocks until at least one byte is written; it does not block until all the bytes in `buffer` is written. To avoid blocking, call this function only if CFWriteStreamCanAcceptBytes(_:) returns `true` or after the stream’s client (set with CFWriteStreamSetClient(_:_:_:_:)) is notified of a canAcceptBytes event.

