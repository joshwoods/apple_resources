

- Core Foundation
-  CFReadStreamUnscheduleFromRunLoop(\_:\_:\_:) 

Function

# CFReadStreamUnscheduleFromRunLoop(\_:\_:\_:)

Removes a read stream from a given run loop.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFReadStreamUnscheduleFromRunLoop(
    _ stream: CFReadStream!,
    _ runLoop: CFRunLoop!,
    _ runLoopMode: CFRunLoopMode!
)
```

## Parameters 

`stream`  

The stream to unschedule.

`runLoop`  

The run loop from which to remove `stream`.

`runLoopMode`  

The run loop mode of `runLoop` from which to remove `stream`.

## See Also

### Scheduling a Read Stream

func CFReadStreamScheduleWithRunLoop(CFReadStream!, CFRunLoop!, CFRunLoopMode!)

Schedules a stream into a run loop.

