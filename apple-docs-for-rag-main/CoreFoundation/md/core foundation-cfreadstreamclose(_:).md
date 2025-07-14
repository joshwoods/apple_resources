

- Core Foundation
-  CFReadStreamClose(\_:) 

Function

# CFReadStreamClose(\_:)

Closes a readable stream.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFReadStreamClose(_ stream: CFReadStream!)
```

## Parameters 

`stream`  

The stream to close.

## Discussion

This function terminates the flow of bytes and releases any system resources required by the stream. The stream is removed from any run loops in which it was scheduled. Once closed, the stream cannot be reopened.

## See Also

### Opening and Closing a Read Stream

func CFReadStreamOpen(CFReadStream!) -> Bool

Opens a stream for reading.

