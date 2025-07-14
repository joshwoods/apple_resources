

- AppKit
- NSFormCell
-  preferredTextFieldWidth 

Instance Property

# preferredTextFieldWidth

The preferred text field width.

macOS 10.8+

``` source
@MainActor
var preferredTextFieldWidth: CGFloat { get set }
```

## Discussion

The preferred width is reflected in the cell’s `cellSize`, which will be large enough to accommodate the title, bezel, and a text field of width `preferredTextWidth`. It is also reflected in the intrinsicContentSize of the NSForm object. That is, under Auto Layout, the form will try to size itself so that the text field cell is the given width, according to the usual content size constraint priorities.

If the width is negative, the cel size matches the historic behavior, which is that it is large enough to accommodate the title, bezel, and the current text.

This property can aid migration to Auto Layout, and is sufficient for simple cases. However, for new apps, it’s recommended that you use an NSTextField instance directly instead of a form.

The default value of this property is `-1`.

