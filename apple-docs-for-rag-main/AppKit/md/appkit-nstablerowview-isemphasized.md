

- AppKit
- NSTableRowView
-  isEmphasized 

Instance Property

# isEmphasized

Determines whether the row will draw with the alternate or secondary color (unless overridden).

macOS 10.7+

``` source
@MainActor
var isEmphasized: Bool { get set }
```

## Discussion

When emphasized is true, the view will draw with the alternateSelectedControlColor defined by NSColor. When false it will use the secondarySelectedControlColor defined by NSColor.

## See Also

### Related Documentation

Table View Programming Guide for Mac

Drag and Drop Programming Topics

### Display Style

var interiorBackgroundStyle: NSView.BackgroundStyle

Specifies how the subviews should draw.

var isFloating: Bool

Specifies whether the row is drawn using the floating style.

