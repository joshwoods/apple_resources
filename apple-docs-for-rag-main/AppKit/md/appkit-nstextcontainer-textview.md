

- AppKit
- NSTextContainer
-  textView 

Instance Property

# textView

The text container’s text view.

macOS

``` source
weak var textView: NSTextView? { get set }
```

## Discussion

A text container doesn’t need a text view to calculate line fragment rectangles, but must have one to display text.

You can use this property to disconnect a text view from a group of text system objects by sending this message to its text container and passing `nil` as `aTextView`.

## See Also

### Managing text components

var layoutManager: NSLayoutManager?

The text container’s layout manager.

var textLayoutManager: NSTextLayoutManager?

func replaceLayoutManager(NSLayoutManager)

Replaces the layout manager for the group of text system objects that contains the text container.

