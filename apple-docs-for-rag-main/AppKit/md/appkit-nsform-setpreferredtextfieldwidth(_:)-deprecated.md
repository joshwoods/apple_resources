

- AppKit
- NSForm
-  setPreferredTextFieldWidth(\_:) Deprecated

Instance Method

# setPreferredTextFieldWidth(\_:)

Sets the preferred text field width used by Auto Layout.

macOS 10.8–10.10Deprecated

``` source
@MainActor
func setPreferredTextFieldWidth(_ preferredWidth: CGFloat)
```

## Parameters 

`preferredWidth`  

The preferred width.

## Discussion

The preferred width is reflected in the cell’s cellSize, which will be large enough to accommodate the title, bezel, and a text field of width preferredTextWidth. It is also reflected in the intrinsicContentSize of the form. That is, under Auto Layout, the form will try to size itself so that the text field cell is the given width, according to the usual content size constraint priorities.

If the width is negative, the cellSize matches the historic behavior, which is that it is large enough to accommodate the title, bezel, and the current text.

The preferred width is reflected in the cell’s cellSize, which will be large enough to accommodate the title, bezel, and a text field of width preferredTextFieldWidth().

This method can aid migration to Auto Layout, and is sufficient for simple cases. However, for new apps, use NSTextField objects directly instead of `NSForm`.

The default is -1.

## See Also

### Auto Layout Sizing

func preferredTextFieldWidth() -> CGFloat

The preferred width of the form’s cells when using Auto Layout.

Deprecated

