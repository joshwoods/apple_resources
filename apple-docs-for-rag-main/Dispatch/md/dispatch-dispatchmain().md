

- Dispatch
-  dispatchMain() 

Function

# dispatchMain()

Executes blocks submitted to the main queue.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func dispatchMain() -> Never
```

## Return Value

This function never returns.

## Discussion

This function “parks” the main thread and waits for blocks to be submitted to the main queue. Applications that call UIApplicationMain(_:_:_:_:) (iOS), NSApplicationMain(_:_:) (macOS), or CFRunLoopRun() on the main thread must not call dispatchMain().

