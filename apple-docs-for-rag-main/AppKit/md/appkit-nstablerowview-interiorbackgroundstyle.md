

- AppKit
- NSTableRowView
-  interiorBackgroundStyle 

Instance Property

# interiorBackgroundStyle

Specifies how the subviews should draw.

macOS 10.7+

``` source
@MainActor
var interiorBackgroundStyle: NSView.BackgroundStyle { get }
```

## Discussion

This value is dynamically computed based on the set of properties set for the `NSTableRowView`.

Subclassers can override this value when they draw differently based on the currently displayed properties.

This property can also be set to determine the color a subview should use. See NSView.BackgroundStyle for supported values.

## See Also

### Display Style

var isEmphasized: Bool

Determines whether the row will draw with the alternate or secondary color (unless overridden).

var isFloating: Bool

Specifies whether the row is drawn using the floating style.

