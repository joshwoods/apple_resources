

- AppKit
- NSTokenFieldCellDelegate
-  tokenFieldCell(\_:shouldAdd:at:) 

Instance Method

# tokenFieldCell(\_:shouldAdd:at:)

Allows the delegate to validate the tokens to be added to the receiver at a given index.

macOS

``` source
@MainActor
optional func tokenFieldCell(
    _ tokenFieldCell: NSTokenFieldCell,
    shouldAdd tokens: [Any],
    at index: Int
) -> [Any]
```

## Parameters 

`tokenFieldCell`  

The token field cell that sent the message.

`tokens`  

An array of tokens to be inserted in the receiver at `index`.

`index`  

The index of the receiver in which the array of tokens to be validated (`tokens`) will be inserted.

## Return Value

An array of validated tokens.

## Discussion

The delegate can return the array unchanged or return a modified array of tokens. To reject the add completely, return an empty array. Returning `nil` causes an error.

## See Also

### Editing a Tokenized Strings

func tokenFieldCell(NSTokenFieldCell, completionsForSubstring: String, indexOfToken: Int, indexOfSelectedItem: UnsafeMutablePointer&lt;Int>) -> [Any]

Allows the delegate to provide an array of appropriate completions for the contents of the receiver.

func tokenFieldCell(NSTokenFieldCell, editingStringForRepresentedObject: Any) -> String?

Allows the delegate to provide a string to be edited as a proxy for the represented object.

func tokenFieldCell(NSTokenFieldCell, representedObjectForEditing: String) -> Any?

Allows the delegate to provide a represented object for the string being edited.

