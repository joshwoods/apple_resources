

- AppKit
- NSDocument
-  showWindows() 

Instance Method

# showWindows()

Displays all of the document’s windows, bringing them to the front and making them main or key as necessary.

macOS

``` source
@MainActor
func showWindows()
```

## See Also

### Managing Document Windows

func setWindow(NSWindow?)

Sets the window outlet of this document to the specified value.

var windowForSheet: NSWindow?

Returns the document window to use as the parent of a document-modal sheet.

var displayName: String!

The name of the document as displayed in the title bars of the document’s windows and in alert dialogs related to the document.

func defaultDraftName() -> String

Returns the default draft name for the document subclass.

func encodeRestorableState(with: NSCoder, backgroundQueue: OperationQueue)

Saves the interface-related state of the document.

