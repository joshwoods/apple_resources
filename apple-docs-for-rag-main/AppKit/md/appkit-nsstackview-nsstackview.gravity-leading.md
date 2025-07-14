

- AppKit
- NSStackView
- NSStackView.Gravity
-  leading 

Type Property

# leading

The leftmost or rightmost gravity area in a horizontally oriented stack view, based on the user interface language or the explicitly set user interface layout direction.

macOS 10.9+

``` source
static var leading: NSStackView.Gravity { get }
```

## Discussion

For a left to right layout direction, the leading gravity area is on the left. Use only when the value of the orientation property is NSUserInterfaceLayoutOrientation.horizontal.

## See Also

### Constants

case top

The topmost gravity area in a vertically oriented stack view.

case center

The center gravity area, regardless of stack view layout direction or user interface language.

case bottom

The bottommost gravity area in a vertically oriented stack view.

static var trailing: NSStackView.Gravity

The leftmost or rightmost gravity area in a horizontally oriented stack view, based on the user interface language or the explicitly set user interface layout direction.

