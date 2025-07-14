

- AppKit
- NSDocument
-  saveTo(\_:) 

Instance Method

# saveTo(\_:)

The action method invoked in the receiver as first responder when the user chooses the Save To menu command.

macOS

``` source
@IBAction @MainActor
func saveTo(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message.

## Discussion

The default implementation is identical to saveAs(_:) except that this method doesn’t clear the document’s edited status and doesn’t reset file location and document type if the document is a native type.

## See Also

### Handling User Actions

func printDocument(Any?)

Prints the receiver in response to the user choosing the Print menu command.

func runPageLayout(Any?)

The action method invoked in the receiver as first responder when the user chooses the Page Setup menu command.

func revertToSaved(Any?)

The action of the File menu item Revert in a document-based app.

func save(Any?)

The action method invoked in the receiver as first responder when the user chooses the Save menu command.

func saveAs(Any?)

The action method invoked in the receiver as first responder when the user chooses the Save As menu command.

func save(withDelegate: Any?, didSave: Selector?, contextInfo: UnsafeMutableRawPointer?)

Saves the document and delivers the results to the provided delegate object.

