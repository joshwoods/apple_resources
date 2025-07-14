

- AppKit
- NSCell
-  endEditing(\_:) 

Instance Method

# endEditing(\_:)

Ends the editing of text in the receiver using the specified field editor.

macOS

``` source
@MainActor
func endEditing(_ textObj: NSText)
```

## Parameters 

`textObj`  

The field editor currently handling the editing of the cell’s content.

## Discussion

Ends any editing of text that began with a call to edit(withFrame:in:editor:delegate:event:) or select(withFrame:in:editor:delegate:start:length:).

## See Also

### Editing and Selecting Text

func edit(withFrame: NSRect, in: NSView, editor: NSText, delegate: Any?, event: NSEvent?)

Begins editing of the receiver’s text using the specified field editor.

func select(withFrame: NSRect, in: NSView, editor: NSText, delegate: Any?, start: Int, length: Int)

Selects the specified text range in the cell’s field editor.

var sendsActionOnEndEditing: Bool

A Boolean value indicating whether the cell’s control object sends its action message when the user finishes editing the cell’s text.

var wantsNotificationForMarkedText: Bool

A Boolean value indicating whether the cell’s field editor should post text change notifications.

func fieldEditor(for: NSView) -> NSTextView?

Returns a custom field editor for editing in the view.

var usesSingleLineMode: Bool

A Boolean value indicating whether the cell restricts layout and rendering of text to a single line.

