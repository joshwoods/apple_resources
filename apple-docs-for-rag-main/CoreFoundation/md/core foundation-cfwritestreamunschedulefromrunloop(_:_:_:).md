

- Core Foundation
-  CFWriteStreamUnscheduleFromRunLoop(\_:\_:\_:) 

Function

# CFWriteStreamUnscheduleFromRunLoop(\_:\_:\_:)

Removes a stream from a particular run loop.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFWriteStreamUnscheduleFromRunLoop(
    _ stream: CFWriteStream!,
    _ runLoop: CFRunLoop!,
    _ runLoopMode: CFRunLoopMode!
)
```

## Parameters 

`stream`  

The stream to remove.

`runLoop`  

The run loop from which to remove `stream`.

`runLoopMode`  

The run loop mode of `runLoop` from which to remove `stream`.

## See Also

### Scheduling a Write Stream

func CFWriteStreamScheduleWithRunLoop(CFWriteStream!, CFRunLoop!, CFRunLoopMode!)

Schedules a stream into a run loop.

