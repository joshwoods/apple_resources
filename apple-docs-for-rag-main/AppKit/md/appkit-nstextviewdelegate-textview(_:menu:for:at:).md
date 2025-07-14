

- AppKit
- NSTextViewDelegate
-  textView(\_:menu:for:at:) 

Instance Method

# textView(\_:menu:for:at:)

Allows delegate to control the context menu returned by the text view.

macOS 10.5+

``` source
@MainActor
optional func textView(
    _ view: NSTextView,
    menu: NSMenu,
    for event: NSEvent,
    at charIndex: Int
) -> NSMenu?
```

## Parameters 

`view`  

The text view sending the message.

`menu`  

The proposed contextual menu.

`event`  

The mouse-down event that initiated the contextual menu’s display.

`charIndex`  

The character position where the mouse button was clicked.

## Return Value

A menu to use as the contextual menu. You can return `menu` unaltered, or you can return a customized menu.

## Discussion

This method allows the delegate to control the context menu returned by menu(for:).

