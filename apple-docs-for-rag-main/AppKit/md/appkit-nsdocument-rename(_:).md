

- AppKit
- NSDocument
-  rename(\_:) 

Instance Method

# rename(\_:)

Renames the current document in response to the user choosing the Rename menu item.

macOS 10.8+

``` source
@IBAction @MainActor
func rename(_ sender: Any?)
```

## Parameters 

`sender`  

The control sending the message.

## Discussion

This is the action method of the Rename menu item in a document-based app. The default implementation of this method initiates a renaming session in a window created by the `[self windowForSheet]` message.

