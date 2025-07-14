

- Core Foundation
-  CFReadStreamScheduleWithRunLoop(\_:\_:\_:) 

Function

# CFReadStreamScheduleWithRunLoop(\_:\_:\_:)

Schedules a stream into a run loop.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFReadStreamScheduleWithRunLoop(
    _ stream: CFReadStream!,
    _ runLoop: CFRunLoop!,
    _ runLoopMode: CFRunLoopMode!
)
```

## Parameters 

`stream`  

The stream to schedule.

`runLoop`  

The run loop with which to schedule `stream`.

`runLoopMode`  

The run loop mode of `runLoop` in which to schedule `stream`.

## Discussion

After scheduling `stream` with a run loop, its client (set with CFReadStreamSetClient(_:_:_:_:)) is notified when various events happen with the stream, such as when it finishes opening, when it has bytes available, and when an error occurs. A stream can be scheduled with multiple run loops and run loop modes. Use CFReadStreamUnscheduleFromRunLoop(_:_:_:) to later remove `stream` from the run loop.

## See Also

### Scheduling a Read Stream

func CFReadStreamUnscheduleFromRunLoop(CFReadStream!, CFRunLoop!, CFRunLoopMode!)

Removes a read stream from a given run loop.

