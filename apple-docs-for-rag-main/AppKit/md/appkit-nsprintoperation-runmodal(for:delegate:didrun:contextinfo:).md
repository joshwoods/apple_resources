

- AppKit
- NSPrintOperation
-  runModal(for:delegate:didRun:contextInfo:) 

Instance Method

# runModal(for:delegate:didRun:contextInfo:)

Runs the print operation, calling your custom delegate method upon completion.

macOS

``` source
@MainActor
func runModal(
    for docWindow: NSWindow,
    delegate: Any?,
    didRun didRunSelector: Selector?,
    contextInfo: UnsafeMutableRawPointer?
)
```

## Parameters 

`docWindow`  

The document window to receive a print progress sheet.

`delegate`  

The printing delegate object. Messages are sent to this object.

`didRunSelector`  

The delegate method called after the completion of the print operation.

`contextInfo`  

A pointer to any data you want passed to the method in the `didRunSelector` parameter.

## Discussion

The method specified by the `didRunSelector` parameter must have the following signature:

```
- (void)printOperationDidRun:(NSPrintOperation *)printOperation  success:(BOOL)success  contextInfo:(void *)contextInfo
```

The value of `success` is true if the print operation ran to completion without cancellation or error, and false otherwise.

If you send canSpawnSeparateThread to an `NSPrintOperation` object with an argument of true, then the delegate specified in a subsequent invocation of runModal(for:delegate:didRun:contextInfo:) may be messaged in that spawned, non-main thread.

## See Also

### Running the Print Operation

func run() -> Bool

Runs the print operation on the current thread.

func cleanUp()

Called at the end of a print operation to remove the print operation as the current operation.

func deliverResult() -> Bool

Delivers the results of the print operation to the intended destination.

