

- Core Foundation
- CFRunLoop
-  CFRunLoopRunInMode Exit Codes 

API Collection

# CFRunLoopRunInMode Exit Codes

Return codes for `CFRunLoopRunInMode`, identifying the reason the run loop exited.

## Topics

### Constants

case finished

The running run loop mode has no sources or timers to process.

case stopped

CFRunLoopStop(_:) was called on the run loop.

case timedOut

The specified time interval for running the run loop has passed.

case handledSource

A source has been processed. This value is returned only if the run loop was told to run only until a source was processed.

## See Also

### Constants

Common Mode Flag

A run loop pseudo-mode that manages objects monitored in the “common” modes.

Default Run Loop Mode

Default run loop mode.

