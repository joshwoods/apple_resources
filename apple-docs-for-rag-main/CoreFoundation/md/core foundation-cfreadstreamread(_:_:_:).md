

- Core Foundation
-  CFReadStreamRead(\_:\_:\_:) 

Function

# CFReadStreamRead(\_:\_:\_:)

Reads data from a readable stream.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFReadStreamRead(
    _ stream: CFReadStream!,
    _ buffer: UnsafeMutablePointer!,
    _ bufferLength: CFIndex
) -> CFIndex
```

## Parameters 

`stream`  

The stream from which to read.

`buffer`  

The buffer into which to place the data.

`bufferLength`  

The size of `buffer` and the maximum number of bytes to read.

## Return Value

The number of bytes read; `0` if the stream has reached its end; or `-1` if either the stream is not open or an error occurs.

## Discussion

If `stream` is in the process of opening, this function waits until it has completed. This function blocks until at least one byte is available; it does not block until `buffer` is filled. To avoid blocking, call this function only if CFReadStreamHasBytesAvailable(_:) returns `TRUE` or after the stream’s client (set with CFReadStreamSetClient(_:_:_:_:)) is notified of a hasBytesAvailable event.

