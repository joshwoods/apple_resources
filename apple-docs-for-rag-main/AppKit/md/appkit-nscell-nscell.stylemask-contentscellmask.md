

- AppKit
- NSCell
- NSCell.StyleMask
-  contentsCellMask 

Type Property

# contentsCellMask

The button cell displays its alternate icon and/or title.

macOS

``` source
static var contentsCellMask: NSCell.StyleMask { get }
```

## See Also

### Constants

static var pushInCellMask: NSCell.StyleMask

The button cell “pushes in” if it has a border.

static var changeGrayCellMask: NSCell.StyleMask

The button cell swaps the “control color” (the controlColor method of `NSColor`) and white pixels on its background and icon.

static var changeBackgroundCellMask: NSCell.StyleMask

Same as `NSChangeGrayCellMask`, but only background pixels are changed.

