

- AppKit
- NSStackView
- NSStackView.Gravity
-  trailing 

Type Property

# trailing

The leftmost or rightmost gravity area in a horizontally oriented stack view, based on the user interface language or the explicitly set user interface layout direction.

macOS 10.9+

``` source
static var trailing: NSStackView.Gravity { get }
```

## Discussion

For a left to right layout direction, the trailing gravity area is on the right. Use only when the value of the orientation property is NSUserInterfaceLayoutOrientation.horizontal.

## See Also

### Constants

case top

The topmost gravity area in a vertically oriented stack view.

static var leading: NSStackView.Gravity

The leftmost or rightmost gravity area in a horizontally oriented stack view, based on the user interface language or the explicitly set user interface layout direction.

case center

The center gravity area, regardless of stack view layout direction or user interface language.

case bottom

The bottommost gravity area in a vertically oriented stack view.

