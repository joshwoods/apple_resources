

- Core Foundation
- CFRunLoopRunResult
-  CFRunLoopRunResult.finished 

Case

# CFRunLoopRunResult.finished

The running run loop mode has no sources or timers to process.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case finished
```

## See Also

### Constants

case stopped

CFRunLoopStop(_:) was called on the run loop.

case timedOut

The specified time interval for running the run loop has passed.

case handledSource

A source has been processed. This value is returned only if the run loop was told to run only until a source was processed.

