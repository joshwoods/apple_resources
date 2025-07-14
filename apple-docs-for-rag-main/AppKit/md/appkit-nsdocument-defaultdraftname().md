

- AppKit
- NSDocument
-  defaultDraftName() 

Instance Method

# defaultDraftName()

Returns the default draft name for the document subclass.

macOS 10.8+

``` source
@MainActor
func defaultDraftName() -> String
```

## Discussion

The default implementation of this method returns the string “Untitled”, as adjusted according to the user’s specified locale. Your app should typically return a name that describes the kind of document. For example, a spreadsheet app could return “Spreadsheet”. A document created from a template could return the name of the template, for example, “Résumé”.

When a document has not yet been assigned a name, and has not yet been autosaved with the NSDocument.SaveOperationType.autosaveAsOperation save operation type, the document bases the default name on the value in the displayName property.

If there is a already another document or file in the same place and with the same name as would be returned by this method, NSDocument appends a number to the defaultDraftName() string.

## See Also

### Managing Document Windows

func showWindows()

Displays all of the document’s windows, bringing them to the front and making them main or key as necessary.

func setWindow(NSWindow?)

Sets the window outlet of this document to the specified value.

var windowForSheet: NSWindow?

Returns the document window to use as the parent of a document-modal sheet.

var displayName: String!

The name of the document as displayed in the title bars of the document’s windows and in alert dialogs related to the document.

func encodeRestorableState(with: NSCoder, backgroundQueue: OperationQueue)

Saves the interface-related state of the document.

