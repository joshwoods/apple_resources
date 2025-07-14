

- AppKit
- NSDocument
-  runPageLayout(\_:) 

Instance Method

# runPageLayout(\_:)

The action method invoked in the receiver as first responder when the user chooses the Page Setup menu command.

macOS

``` source
@IBAction @MainActor
func runPageLayout(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message.

## Discussion

The default implementation invokes runModalPageLayout(with:delegate:didRun:contextInfo:) with the document’s current NSPrintInfo object as argument; if the user clicks the OK button and the document authorizes changes to its printing information (shouldChangePrintInfo(_:)), the method sets the document’s new `NSPrintInfo` object and increments the document’s change count.

## See Also

### Related Documentation

func updateChangeCount(NSDocument.ChangeType)

Updates the receiver’s change count according to the given change type.

var printInfo: NSPrintInfo

The printing information associated with the document.

### Handling User Actions

func printDocument(Any?)

Prints the receiver in response to the user choosing the Print menu command.

func revertToSaved(Any?)

The action of the File menu item Revert in a document-based app.

func save(Any?)

The action method invoked in the receiver as first responder when the user chooses the Save menu command.

func saveAs(Any?)

The action method invoked in the receiver as first responder when the user chooses the Save As menu command.

func saveTo(Any?)

The action method invoked in the receiver as first responder when the user chooses the Save To menu command.

func save(withDelegate: Any?, didSave: Selector?, contextInfo: UnsafeMutableRawPointer?)

Saves the document and delivers the results to the provided delegate object.

