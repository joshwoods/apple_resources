

- AppKit
- NSDocumentController
-  saveAllDocuments(\_:) 

Instance Method

# saveAllDocuments(\_:)

As the action method called by the Save All command, saves all open documents of the application that need to be saved.

macOS

``` source
@IBAction @MainActor
func saveAllDocuments(_ sender: Any?)
```

## See Also

### Related Documentation

func save(Any?)

The action method invoked in the receiver as first responder when the user chooses the Save menu command.

### Responding to Action Messages

func newDocument(Any?)

An action method called by the New menu command, this method creates a new `NSDocument` object and adds it to the list of such objects managed by the document controller.

func openDocument(Any?)

An action method called by the Open menu command, it runs the modal Open panel and, based on the selected filenames, creates one or more `NSDocument` objects from the contents of the files.

