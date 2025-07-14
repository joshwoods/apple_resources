

- AppKit
- NSDocumentController
-  openDocument(\_:) 

Instance Method

# openDocument(\_:)

An action method called by the Open menu command, it runs the modal Open panel and, based on the selected filenames, creates one or more `NSDocument` objects from the contents of the files.

macOS

``` source
@IBAction @MainActor
func openDocument(_ sender: Any?)
```

## Discussion

The method adds the newly created objects to the list of `NSDocument` objects managed by the document controller. This method calls openDocument(withContentsOf:display:completionHandler:), which actually creates the `NSDocument` objects.

## See Also

### Responding to Action Messages

func newDocument(Any?)

An action method called by the New menu command, this method creates a new `NSDocument` object and adds it to the list of such objects managed by the document controller.

func saveAllDocuments(Any?)

As the action method called by the Save All command, saves all open documents of the application that need to be saved.

