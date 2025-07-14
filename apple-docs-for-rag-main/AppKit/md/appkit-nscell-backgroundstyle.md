

- AppKit
- NSCell
-  backgroundStyle 

Instance Property

# backgroundStyle

The cell’s background style.

macOS 10.5+

``` source
@MainActor
var backgroundStyle: NSView.BackgroundStyle { get set }
```

## Discussion

The background describes the surface the cell is drawn onto in the draw(withFrame:in:) method. A control typically sets the value of this property before it asks the cell to draw. A cell may draw differently based on background characteristics. For example, a table view drawing a cell in a selected row might set the value to dark. A text cell might decide to render its text white as a result. A rating-style level indicator might draw its stars white instead of gray.

## See Also

### Managing Display Attributes

var isBezeled: Bool

A Boolean value indicating whether the cell has a bezeled border.

var isBordered: Bool

A Boolean value indicating whether the cell draws itself outlined with a plain border.

var isOpaque: Bool

A Boolean value indicating whether the cell is completely opaque.

var controlTint: NSControlTint

The cell’s control tint.

Deprecated

var interiorBackgroundStyle: NSView.BackgroundStyle

The cell’s interior background style.

enum BackgroundStyle

Background styles to apply to a view’s cell.

