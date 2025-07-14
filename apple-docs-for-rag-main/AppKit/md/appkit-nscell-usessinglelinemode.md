

- AppKit
- NSCell
-  usesSingleLineMode 

Instance Property

# usesSingleLineMode

A Boolean value indicating whether the cell restricts layout and rendering of text to a single line.

macOS 10.6+

``` source
@MainActor
var usesSingleLineMode: Bool { get set }
```

## Discussion

When the value of this property is true, text layout and rendering is restricted to a single line. In addition, the cell ignores the return value from wraps, interprets NSLineBreakMode.byWordWrapping and NSLineBreakMode.byCharWrapping returned by lineBreakMode as NSLineBreakMode.byClipping, and configures the field editor to ignore key binding commands that insert paragraph and line separators.

The field editor bound to a single-line cell filters out paragraph and line separator insertion from user actions. Cells in single-line mode use the fixed baseline layout. The text baseline position is determined solely by the control size regardless of content font style or size.

## See Also

### Editing and Selecting Text

func edit(withFrame: NSRect, in: NSView, editor: NSText, delegate: Any?, event: NSEvent?)

Begins editing of the receiver’s text using the specified field editor.

func select(withFrame: NSRect, in: NSView, editor: NSText, delegate: Any?, start: Int, length: Int)

Selects the specified text range in the cell’s field editor.

var sendsActionOnEndEditing: Bool

A Boolean value indicating whether the cell’s control object sends its action message when the user finishes editing the cell’s text.

func endEditing(NSText)

Ends the editing of text in the receiver using the specified field editor.

var wantsNotificationForMarkedText: Bool

A Boolean value indicating whether the cell’s field editor should post text change notifications.

func fieldEditor(for: NSView) -> NSTextView?

Returns a custom field editor for editing in the view.

