

- AppKit
- NSDocumentController
-  newDocument(\_:) 

Instance Method

# newDocument(\_:)

An action method called by the New menu command, this method creates a new `NSDocument` object and adds it to the list of such objects managed by the document controller.

macOS

``` source
@IBAction @MainActor
func newDocument(_ sender: Any?)
```

## Discussion

This method calls openUntitledDocumentAndDisplay(_:).

## See Also

### Responding to Action Messages

func openDocument(Any?)

An action method called by the Open menu command, it runs the modal Open panel and, based on the selected filenames, creates one or more `NSDocument` objects from the contents of the files.

func saveAllDocuments(Any?)

As the action method called by the Save All command, saves all open documents of the application that need to be saved.

