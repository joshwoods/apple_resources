

- Core Foundation
-  CFWriteStreamOpen(\_:) 

Function

# CFWriteStreamOpen(\_:)

Opens a stream for writing.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFWriteStreamOpen(_ stream: CFWriteStream!) -> Bool
```

## Parameters 

`stream`  

The stream to open.

## Return Value

`true` if `stream` was successfully opened, `false` otherwise. If `stream` is not in the CFStreamStatus.notOpen state, this function returns `false`.

## Discussion

Opening a stream causes it to reserve all the system resources it requires. If the stream can open in the background without blocking, this function always returns `true`. To learn when a background open operation completes, you can either schedule the stream into a run loop with CFWriteStreamScheduleWithRunLoop(_:_:_:) and wait for the stream’s client (set with CFWriteStreamSetClient(_:_:_:_:)) to be notified or you can poll the stream using CFWriteStreamGetStatus(_:), waiting for a status of CFStreamStatus.open or CFStreamStatus.error.

## See Also

### Opening and Closing a Stream

func CFWriteStreamClose(CFWriteStream!)

Closes a writable stream.

