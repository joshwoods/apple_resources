

- AppKit
- NSForm
-  preferredTextFieldWidth() Deprecated

Instance Method

# preferredTextFieldWidth()

The preferred width of the form’s cells when using Auto Layout.

macOS 10.8–10.10Deprecated

``` source
@MainActor
func preferredTextFieldWidth() -> CGFloat
```

## Return Value

The field’s width.

## Discussion

If the width is negative, the cellSize matches the historic behavior, which is that it is large enough to accommodate the title, bezel, and the current text.

The default is -1.

## See Also

### Auto Layout Sizing

func setPreferredTextFieldWidth(CGFloat)

Sets the preferred text field width used by Auto Layout.

Deprecated

