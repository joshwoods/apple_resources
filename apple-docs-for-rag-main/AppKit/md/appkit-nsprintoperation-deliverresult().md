

- AppKit
- NSPrintOperation
-  deliverResult() 

Instance Method

# deliverResult()

Delivers the results of the print operation to the intended destination.

macOS

``` source
@MainActor
func deliverResult() -> Bool
```

## Return Value

true if the results were successfully delivered; otherwise, false.

## Discussion

This method may be called to deliver the results to the printer spool or preview application. Do not invoke this method directly—it is invoked automatically when the print operation is done.

## See Also

### Running the Print Operation

func run() -> Bool

Runs the print operation on the current thread.

func runModal(for: NSWindow, delegate: Any?, didRun: Selector?, contextInfo: UnsafeMutableRawPointer?)

Runs the print operation, calling your custom delegate method upon completion.

func cleanUp()

Called at the end of a print operation to remove the print operation as the current operation.

