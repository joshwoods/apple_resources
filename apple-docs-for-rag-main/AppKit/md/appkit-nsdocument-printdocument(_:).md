

- AppKit
- NSDocument
-  printDocument(\_:) 

Instance Method

# printDocument(\_:)

Prints the receiver in response to the user choosing the Print menu command.

macOS

``` source
@IBAction @MainActor
func printDocument(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message.

## Discussion

An `NSDocument` object receives this action message as it travels up the responder chain. The default implementation invokes print(withSettings:showPrintPanel:delegate:didPrint:contextInfo:).

## See Also

### Related Documentation

var printInfo: NSPrintInfo

The printing information associated with the document.

func shouldChangePrintInfo(NSPrintInfo) -> Bool

Returns a Boolean value that indicates whether the document allows changes to the default printing information.

### Handling User Actions

func runPageLayout(Any?)

The action method invoked in the receiver as first responder when the user chooses the Page Setup menu command.

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

