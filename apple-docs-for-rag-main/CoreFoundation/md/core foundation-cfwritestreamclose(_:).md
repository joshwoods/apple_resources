

- Core Foundation
-  CFWriteStreamClose(\_:) 

Function

# CFWriteStreamClose(\_:)

Closes a writable stream.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFWriteStreamClose(_ stream: CFWriteStream!)
```

## Parameters 

`stream`  

The stream to close.

## Discussion

This function terminates the flow of bytes and releases any system resources required by the stream. The stream is removed from any run loops in which it was scheduled. Once closed, the stream cannot be reopened.

## See Also

### Opening and Closing a Stream

func CFWriteStreamOpen(CFWriteStream!) -> Bool

Opens a stream for writing.

