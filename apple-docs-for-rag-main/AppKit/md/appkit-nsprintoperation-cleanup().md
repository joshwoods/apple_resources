

- AppKit
- NSPrintOperation
-  cleanUp() 

Instance Method

# cleanUp()

Called at the end of a print operation to remove the print operation as the current operation.

macOS

``` source
@MainActor
func cleanUp()
```

## Discussion

You typically do not invoke this method directly.

## See Also

### Running the Print Operation

func run() -> Bool

Runs the print operation on the current thread.

func runModal(for: NSWindow, delegate: Any?, didRun: Selector?, contextInfo: UnsafeMutableRawPointer?)

Runs the print operation, calling your custom delegate method upon completion.

func deliverResult() -> Bool

Delivers the results of the print operation to the intended destination.

