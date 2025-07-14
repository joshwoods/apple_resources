

- Core Foundation
-  CFRunLoopTimerCallBack 

Type Alias

# CFRunLoopTimerCallBack

Callback invoked when a CFRunLoopTimer object fires.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFRunLoopTimerCallBack = (CFRunLoopTimer?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`timer`  

The run loop timer that is firing.

`info`  

The `info` member of the CFRunLoopTimerContext structure that was used when creating the run loop timer.

## Discussion

If `timer` repeats, the run loop automatically schedules the next firing time after calling this function, unless you manually update the firing time within this callback by calling CFRunLoopTimerSetNextFireDate(_:_:). If `timer` does not repeat, the run loop invalidates `timer`.

You specify this callback when you create the timer with CFRunLoopTimerCreate(_:_:_:_:_:_:_:).

