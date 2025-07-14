

- AppKit
- NSTokenFieldCellDelegate
-  tokenFieldCell(\_:editingStringForRepresentedObject:) 

Instance Method

# tokenFieldCell(\_:editingStringForRepresentedObject:)

Allows the delegate to provide a string to be edited as a proxy for the represented object.

macOS

``` source
@MainActor
optional func tokenFieldCell(
    _ tokenFieldCell: NSTokenFieldCell,
    editingStringForRepresentedObject representedObject: Any
) -> String?
```

## Parameters 

`tokenFieldCell`  

The token field cell that sent the message.

`representedObject`  

A represented object of the token field.

## Return Value

A string that’s an editable proxy of the represented object, or `nil` if the token should not be editable.

## See Also

### Editing a Tokenized Strings

func tokenFieldCell(NSTokenFieldCell, completionsForSubstring: String, indexOfToken: Int, indexOfSelectedItem: UnsafeMutablePointer&lt;Int>) -> [Any]

Allows the delegate to provide an array of appropriate completions for the contents of the receiver.

func tokenFieldCell(NSTokenFieldCell, representedObjectForEditing: String) -> Any?

Allows the delegate to provide a represented object for the string being edited.

func tokenFieldCell(NSTokenFieldCell, shouldAdd: [Any], at: Int) -> [Any]

Allows the delegate to validate the tokens to be added to the receiver at a given index.

