

- AppKit
- NSCell
- NSCell.StyleMask
-  changeBackgroundCellMask 

Type Property

# changeBackgroundCellMask

Same as `NSChangeGrayCellMask`, but only background pixels are changed.

macOS

``` source
static var changeBackgroundCellMask: NSCell.StyleMask { get }
```

## See Also

### Constants

static var pushInCellMask: NSCell.StyleMask

The button cell “pushes in” if it has a border.

static var contentsCellMask: NSCell.StyleMask

The button cell displays its alternate icon and/or title.

static var changeGrayCellMask: NSCell.StyleMask

The button cell swaps the “control color” (the controlColor method of `NSColor`) and white pixels on its background and icon.

