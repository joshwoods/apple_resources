

- AppKit
- NSTextFieldCell
-  setUpFieldEditorAttributes(\_:) 

Instance Method

# setUpFieldEditorAttributes(\_:)

Allows the cell to set up the field editor’s attributes before editing begins.

macOS

``` source
@MainActor
func setUpFieldEditorAttributes(_ textObj: NSText) -> NSText
```

## Parameters 

`textObj`  

A text object configured as a field editor.

## Return Value

A text object with customized attributes suitable for editing the text field cell’s content.

## Discussion

You never invoke this method directly; by overriding it, however, you can customize the field editor. When you override this method, you should generally invoke the implementation of `super` and return the `textObj` argument. For information on field editors, see Using the Window’s Field Editor.

## See Also

### Managing the Field Editor

func setWantsNotificationForMarkedText(Bool)

Directs the cell’s associated field editor to post text change notifications.

