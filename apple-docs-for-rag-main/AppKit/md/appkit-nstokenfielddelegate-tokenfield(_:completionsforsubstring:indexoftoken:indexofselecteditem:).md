

- AppKit
- NSTokenFieldDelegate
-  tokenField(\_:completionsForSubstring:indexOfToken:indexOfSelectedItem:) 

Instance Method

# tokenField(\_:completionsForSubstring:indexOfToken:indexOfSelectedItem:)

Allows the delegate to provide an array of appropriate completions for the contents of the receiver.

macOS

``` source
@MainActor
optional func tokenField(
    _ tokenField: NSTokenField,
    completionsForSubstring substring: String,
    indexOfToken tokenIndex: Int,
    indexOfSelectedItem selectedIndex: UnsafeMutablePointer?
) -> [Any]?
```

## Parameters 

`tokenField`  

The token field where editing is occurring.

`substring`  

The partial string that is to be completed.

`tokenIndex`  

The index of the token being edited.

`selectedIndex`  

Optionally, you can return by-reference an index into the returned array that specifies which of the completions should be initially selected. If none are to be selected, return by reference `-1`.

## Return Value

An array of strings that are possible completions.

## Discussion

If the delegate does not implement this method, no completions are provided.

## See Also

### Editing a Tokenized Strings

func tokenField(NSTokenField, editingStringForRepresentedObject: Any) -> String?

Allows the delegate to provide a string to be edited as a proxy for a represented object.

func tokenField(NSTokenField, representedObjectForEditing: String) -> Any?

Allows the delegate to provide a represented object for the given editing string.

func tokenField(NSTokenField, shouldAdd: [Any], at: Int) -> [Any]

Allows the delegate to validate the tokens to be added to the receiver at a particular location.

