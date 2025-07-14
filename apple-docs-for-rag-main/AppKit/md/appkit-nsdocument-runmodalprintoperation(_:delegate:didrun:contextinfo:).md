

- AppKit
- NSDocument
-  runModalPrintOperation(\_:delegate:didRun:contextInfo:) 

Instance Method

# runModalPrintOperation(\_:delegate:didRun:contextInfo:)

Runs the specified print operation modally.

macOS

``` source
@MainActor
func runModalPrintOperation(
    _ printOperation: NSPrintOperation,
    delegate: Any?,
    didRun didRunSelector: Selector?,
    contextInfo: UnsafeMutableRawPointer?
)
```

## Parameters 

`printOperation`  

The print operation to run.

`delegate`  

The delegate to which the selector message is sent.

`didRunSelector`  

The selector of the message sent to the delegate.

`contextInfo`  

Object passed with the callback to provide any additional context information.

## Discussion

Overrides of printShowingPrintPanel: can invoke this method.

When the panel is dismissed, `delegate` is sent a `didRunSelector` message. Pass the `contextInfo` object with the callback. The `didRunSelector` callback method should have the following signature:

```
- (void)documentDidRunModalPrintOperation:(NSDocument *)document  success:(BOOL)success  contextInfo:(void *)contextInfo
```

## See Also

### Printing the Document

var printInfo: NSPrintInfo

The printing information associated with the document.

func preparePageLayout(NSPageLayout) -> Bool

Adds document-specific content to the Page Layout panel.

func runModalPageLayout(with: NSPrintInfo, delegate: Any?, didRun: Selector?, contextInfo: UnsafeMutableRawPointer?)

Runs the modal page layout panel with the receiver’s printing information object.

func shouldChangePrintInfo(NSPrintInfo) -> Bool

Returns a Boolean value that indicates whether the document allows changes to the default printing information.

func print(withSettings: [NSPrintInfo.AttributeKey : Any], showPrintPanel: Bool, delegate: Any?, didPrint: Selector?, contextInfo: UnsafeMutableRawPointer?)

Prints the document’s contents, optionally displaying a print panel to the user.

func printOperation(withSettings: [NSPrintInfo.AttributeKey : Any]) throws -> NSPrintOperation

Creates and returns a print operation for the document’s contents.

var pdfPrintOperation: NSPrintOperation

A print operation you can use to create a PDF representation of the document’s current contents.

func saveToPDF(Any?)

Exports a PDF representation of the document’s current contents.

