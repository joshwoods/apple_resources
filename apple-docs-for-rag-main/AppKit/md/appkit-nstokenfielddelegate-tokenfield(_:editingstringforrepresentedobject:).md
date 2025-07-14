

- AppKit
- NSTokenFieldDelegate
-  tokenField(\_:editingStringForRepresentedObject:) 

Instance Method

# tokenField(\_:editingStringForRepresentedObject:)

Allows the delegate to provide a string to be edited as a proxy for a represented object.

macOS

``` source
@MainActor
optional func tokenField(
    _ tokenField: NSTokenField,
    editingStringForRepresentedObject representedObject: Any
) -> String?
```

## Parameters 

`tokenField`  

The token field that sent the message.

`representedObject`  

A represented object of the token field.

## Return Value

A string that’s an editable proxy of the represented object, or `nil` if the token should not be editable.

## See Also

### Editing a Tokenized Strings

func tokenField(NSTokenField, completionsForSubstring: String, indexOfToken: Int, indexOfSelectedItem: UnsafeMutablePointer&lt;Int>?) -> [Any]?

Allows the delegate to provide an array of appropriate completions for the contents of the receiver.

func tokenField(NSTokenField, representedObjectForEditing: String) -> Any?

Allows the delegate to provide a represented object for the given editing string.

func tokenField(NSTokenField, shouldAdd: [Any], at: Int) -> [Any]

Allows the delegate to validate the tokens to be added to the receiver at a particular location.

