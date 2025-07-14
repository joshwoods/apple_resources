

- AppKit
- NSTableRowView
-  isFloating 

Instance Property

# isFloating

Specifies whether the row is drawn using the floating style.

macOS 10.7+

``` source
@MainActor
var isFloating: Bool { get set }
```

## Discussion

Floating is a temporary attribute that is set when a particular group row is actually floating above other rows. The state may change dynamically based on the position of the group row. Drawing may be different for rows that are currently ‘floating’.

## See Also

### Display Style

var isEmphasized: Bool

Determines whether the row will draw with the alternate or secondary color (unless overridden).

var interiorBackgroundStyle: NSView.BackgroundStyle

Specifies how the subviews should draw.

