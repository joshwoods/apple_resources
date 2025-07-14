

- AppKit
- NSTokenFieldDelegate
-  tokenField(\_:shouldAdd:at:) 

Instance Method

# tokenField(\_:shouldAdd:at:)

Allows the delegate to validate the tokens to be added to the receiver at a particular location.

macOS

``` source
@MainActor
optional func tokenField(
    _ tokenField: NSTokenField,
    shouldAdd tokens: [Any],
    at index: Int
) -> [Any]
```

## Parameters 

`tokenField`  

The token field that sent the message.

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

func tokenField(NSTokenField, completionsForSubstring: String, indexOfToken: Int, indexOfSelectedItem: UnsafeMutablePointer&lt;Int>?) -> [Any]?

Allows the delegate to provide an array of appropriate completions for the contents of the receiver.

func tokenField(NSTokenField, editingStringForRepresentedObject: Any) -> String?

Allows the delegate to provide a string to be edited as a proxy for a represented object.

func tokenField(NSTokenField, representedObjectForEditing: String) -> Any?

Allows the delegate to provide a represented object for the given editing string.

