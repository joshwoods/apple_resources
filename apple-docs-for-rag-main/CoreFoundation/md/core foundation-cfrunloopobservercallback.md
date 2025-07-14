

- Core Foundation
-  CFRunLoopObserverCallBack 

Type Alias

# CFRunLoopObserverCallBack

Callback invoked when a CFRunLoopObserver object is fired.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFRunLoopObserverCallBack = (CFRunLoopObserver?, CFRunLoopActivity, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`observer`  

The run loop observer that is firing.

`activity`  

The current activity stage of the run loop.

`info`  

The `info` member of the CFRunLoopObserverContext structure that was used when creating the run loop observer.

## Discussion

You specify this callback when you create the run loop observer with CFRunLoopObserverCreate(_:_:_:_:_:_:).

