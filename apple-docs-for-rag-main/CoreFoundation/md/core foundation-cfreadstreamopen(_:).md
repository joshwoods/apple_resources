

- Core Foundation
-  CFReadStreamOpen(\_:) 

Function

# CFReadStreamOpen(\_:)

Opens a stream for reading.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFReadStreamOpen(_ stream: CFReadStream!) -> Bool
```

## Parameters 

`stream`  

The stream to open.

## Return Value

`TRUE` if `stream` was successfully opened, `FALSE` otherwise. If `stream` is not in the CFStreamStatus.notOpen state, this function returns `FALSE`.

## Discussion

Opening a stream causes it to reserve all the system resources it requires. If the stream can open in the background without blocking, this function always returns `true`. To learn when a background open operation completes, you can either schedule the stream into a run loop with CFReadStreamScheduleWithRunLoop(_:_:_:) and wait for the stream’s client (set with CFReadStreamSetClient(_:_:_:_:)) to be notified or you can poll the stream using CFReadStreamGetStatus(_:), waiting for a status of CFStreamStatus.open or CFStreamStatus.error.

You do not need to wait until a stream has finished opening in the background before calling the CFReadStreamRead(_:_:_:) function. The read operation will simply block until the open has completed.

## See Also

### Opening and Closing a Read Stream

func CFReadStreamClose(CFReadStream!)

Closes a readable stream.

