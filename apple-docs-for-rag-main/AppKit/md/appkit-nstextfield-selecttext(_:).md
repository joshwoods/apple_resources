

- AppKit
- NSTextField
-  selectText(\_:) 

Instance Method

# selectText(\_:)

Ends editing in the text field and, if it’s selectable, selects the entire text content.

macOS

``` source
@MainActor
func selectText(_ sender: Any?)
```

## Parameters 

`sender`  

The sender of the message.

## Discussion

If the text field isn’t in a window’s view hierarchy, this method has no effect.

