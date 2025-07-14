

- AppKit
- NSDocument
-  setWindow(\_:) 

Instance Method

# setWindow(\_:)

Sets the window outlet of this document to the specified value.

macOS

``` source
@MainActor
func setWindow(_ window: NSWindow?)
```

## Parameters 

`window`  

The window to which the receiver’s `window` outlet points.

## Discussion

This method is invoked automatically during the loading of any nib for which this document is the file’s owner, if the file’s owner `window` outlet is connected in the nib. You should not invoke this method directly, and typically you would not override it either.

## See Also

### Managing Document Windows

func showWindows()

Displays all of the document’s windows, bringing them to the front and making them main or key as necessary.

var windowForSheet: NSWindow?

Returns the document window to use as the parent of a document-modal sheet.

var displayName: String!

The name of the document as displayed in the title bars of the document’s windows and in alert dialogs related to the document.

func defaultDraftName() -> String

Returns the default draft name for the document subclass.

func encodeRestorableState(with: NSCoder, backgroundQueue: OperationQueue)

Saves the interface-related state of the document.

