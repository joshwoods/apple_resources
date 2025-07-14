

- AppKit
- NSTextSuggestionsDelegate
-  textField(\_:didSelect:) 

Instance Method

# textField(\_:didSelect:)

Called when an item in the suggestions menu has been selected.

macOS 15.0+

``` source
@MainActor
func textField(
    _ textField: NSTextField,
    didSelect item: Self.Item
)
```

**Required** Default implementation provided.

## Parameters 

`textField`  

The text field whose suggestions item was highlighted.

`item`  

The item that was selected.

## Discussion

The default implementation inserts the item’s text completion (`textField(_:textCompletionFor:)`) into the control, replacing its existing text. Overriding this method allows you to do a custom behavior instead.

## Default Implementations

### NSTextSuggestionsDelegate Implementations

func textField(NSTextField, didSelect: Self.Item)

Called when an item in the suggestions menu has been selected.

