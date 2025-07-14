

- AppKit
- NSPrintOperation
-  canSpawnSeparateThread 

Instance Property

# canSpawnSeparateThread

A Boolean value that determines whether the print operation is allowed to spawn a separate printing thread.

macOS

``` source
@MainActor
var canSpawnSeparateThread: Bool { get set }
```

## Parameters 

`canSpawnSeparateThread`  

true if the receiver is allowed to spawn a separate thread; otherwise, false.

## Discussion

If `canSpawnSeparateThread` is true, an `NSThread` object is detached when the print panel is dismissed (or immediately, if the panel is not to be displayed). The new thread performs the print operation, so that control can return to your application. A thread is detached only if the print operation is run using the runModal(for:delegate:didRun:contextInfo:) method. If `canSpawnSeparateThread` is false, the operation runs on the current thread, blocking the application until the operation completes.

If you send canSpawnSeparateThread to an `NSPrintOperation` object with an argument of true, then the delegate specified in a subsequent invocation of runModal(for:delegate:didRun:contextInfo:) may be messaged in that spawned, non-main thread.

