

- AppKit
- NSDocument
-  revertToSaved(\_:) 

Instance Method

# revertToSaved(\_:)

The action of the File menu item Revert in a document-based app.

macOS

``` source
@IBAction @MainActor
func revertToSaved(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message.

## Discussion

The default implementation of this method presents an alert dialog giving the user the opportunity to cancel the operation. If the user chooses to continue, the method ensures that any editor registered using the Cocoa Bindings `NSEditorRegistration` informal protocol has discarded its changes and then invokes revert(toContentsOf:ofType:). If that returns false, the method presents the error to the user in an document-modal alert dialog.

## See Also

### Related Documentation

func updateChangeCount(NSDocument.ChangeType)

Updates the receiver’s change count according to the given change type.

### Handling User Actions

func printDocument(Any?)

Prints the receiver in response to the user choosing the Print menu command.

func runPageLayout(Any?)

The action method invoked in the receiver as first responder when the user chooses the Page Setup menu command.

func save(Any?)

The action method invoked in the receiver as first responder when the user chooses the Save menu command.

func saveAs(Any?)

The action method invoked in the receiver as first responder when the user chooses the Save As menu command.

func saveTo(Any?)

The action method invoked in the receiver as first responder when the user chooses the Save To menu command.

func save(withDelegate: Any?, didSave: Selector?, contextInfo: UnsafeMutableRawPointer?)

Saves the document and delivers the results to the provided delegate object.

