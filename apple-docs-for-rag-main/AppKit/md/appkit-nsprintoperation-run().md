

- AppKit
- NSPrintOperation
-  run() 

Instance Method

# run()

Runs the print operation on the current thread.

macOS

``` source
@MainActor
func run() -> Bool
```

## Return Value

true if the operation was successful; otherwise, false.

## Discussion

The operation runs to completion in the current thread, blocking the application. A separate thread is not spawned, even if canSpawnSeparateThread is true. Use runModal(for:delegate:didRun:contextInfo:) to use document-modal sheets and to allow a separate thread to perform the operation.

## See Also

### Running the Print Operation

func runModal(for: NSWindow, delegate: Any?, didRun: Selector?, contextInfo: UnsafeMutableRawPointer?)

Runs the print operation, calling your custom delegate method upon completion.

func cleanUp()

Called at the end of a print operation to remove the print operation as the current operation.

func deliverResult() -> Bool

Delivers the results of the print operation to the intended destination.

