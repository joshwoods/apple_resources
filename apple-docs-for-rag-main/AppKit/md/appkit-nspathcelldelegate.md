

- AppKit
-  NSPathCellDelegate 

Protocol

# NSPathCellDelegate

A set of methods that enable the delegate of a path cell object to customize the Open panel or pop-up menu of a path whose style is set to NSPathControl.Style.popUp.

macOS

``` source
protocol NSPathCellDelegate : NSObjectProtocol
```

## Topics

### Customizing the Open Panel

func pathCell(NSPathCell, willDisplay: NSOpenPanel)

Implement this method to customize the Open panel shown by a pop-up–style path.

### Customizing the Menu

func pathCell(NSPathCell, willPopUp: NSMenu)

Implement this method to customize the menu of a pop-up–style path.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Cells

class NSPathCell

The user interface of a path control object.

class NSPathComponentCell

A component of a path.

class NSPathControlItem

