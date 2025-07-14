

- Core Foundation
-  CFWriteStreamScheduleWithRunLoop(\_:\_:\_:) 

Function

# CFWriteStreamScheduleWithRunLoop(\_:\_:\_:)

Schedules a stream into a run loop.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFWriteStreamScheduleWithRunLoop(
    _ stream: CFWriteStream!,
    _ runLoop: CFRunLoop!,
    _ runLoopMode: CFRunLoopMode!
)
```

## Parameters 

`stream`  

The stream to schedule.

`runLoop`  

The run loop in which to schedule `stream`.

`runLoopMode`  

The run loop mode of `runLoop` in which to schedule `stream`.

## Discussion

After scheduling `stream` into a run loop, its client (set with CFWriteStreamSetClient(_:_:_:_:)) is notified when various events happen with the stream, such as when it finishes opening, when it can accept new bytes, and when an error occurs. A stream can be scheduled into multiple run loops and run loop modes. Use CFWriteStreamUnscheduleFromRunLoop(_:_:_:) to later remove `stream` from the run loop.

## See Also

### Scheduling a Write Stream

func CFWriteStreamUnscheduleFromRunLoop(CFWriteStream!, CFRunLoop!, CFRunLoopMode!)

Removes a stream from a particular run loop.

