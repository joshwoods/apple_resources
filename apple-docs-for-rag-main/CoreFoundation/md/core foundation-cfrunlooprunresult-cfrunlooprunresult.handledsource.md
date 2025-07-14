

- Core Foundation
- CFRunLoopRunResult
-  CFRunLoopRunResult.handledSource 

Case

# CFRunLoopRunResult.handledSource

A source has been processed. This value is returned only if the run loop was told to run only until a source was processed.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case handledSource
```

## See Also

### Constants

case finished

The running run loop mode has no sources or timers to process.

case stopped

CFRunLoopStop(_:) was called on the run loop.

case timedOut

The specified time interval for running the run loop has passed.

