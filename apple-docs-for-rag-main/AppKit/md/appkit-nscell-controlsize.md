

- AppKit
- NSCell
-  controlSize 

Instance Property

# controlSize

The size of the cell.

macOS

``` source
@MainActor
var controlSize: NSControl.ControlSize { get set }
```

## Discussion

Use this property to change the rendered size of the cell and its control. For a list of possible values, see NSControl.ControlSize.

Changing the cell’s control size does not change the font used by the cell. Use the systemFontSize(for:) class method of NSFont to obtain an appropriate font based on the new control size.

## See Also

### Determining Cell Size

func calcDrawInfo(NSRect)

Recalculates the cell geometry.

var cellSize: NSSize

The minimum size needed to display the cell.

func cellSize(forBounds: NSRect) -> NSSize

Returns the minimum size needed to display the receiver, constraining it to the specified rectangle.

func drawingRect(forBounds: NSRect) -> NSRect

Returns the rectangle within which the receiver draws itself

func imageRect(forBounds: NSRect) -> NSRect

Returns the rectangle in which the receiver draws its image.

func titleRect(forBounds: NSRect) -> NSRect

Returns the rectangle in which the receiver draws its title text.

