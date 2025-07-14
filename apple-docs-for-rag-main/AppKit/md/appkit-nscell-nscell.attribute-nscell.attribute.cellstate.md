

- AppKit
- NSCell
- NSCell.Attribute
-  NSCell.Attribute.cellState 

Case

# NSCell.Attribute.cellState

The cell’s state.

macOS

``` source
case cellState
```

## Discussion

The cell’s state can be NSMixedState, NSOffState, or NSOnState.

## See Also

### Constants

case cellAllowsMixedState

Lets the cell’s state be `NSMixedState`, as well as `NSOffState` and `NSOnState`.

case changeBackgroundCell

If the cell’s state is `NSMixedState` or `NSOnState`, changes the cell’s background color from gray to white.

case cellChangesContents

If the cell’s state is `NSMixedState` or `NSOnState`, displays the cell’s alternate image.

case changeGrayCell

If the cell’s state is `NSMixedState` or `NSOnState`, displays the cell’s image as darkened.

case cellDisabled

Does not let the user manipulate the cell.

case cellEditable

Lets the user edit the cell’s contents.

case cellHasImageHorizontal

Controls the position of the cell’s image: places the image on the right of any text in the cell.

case cellHasImageOnLeftOrBottom

Controls the position of the cell’s image: places the image on the left of or below any text in the cell.

case cellHasOverlappingImage

Controls the position of the cell’s image: places the image over any text in the cell.

case cellHighlighted

Draws the cell with a highlighted appearance.

Deprecated

case cellIsBordered

Draws a border around the cell.

case cellIsInsetButton

Insets the cell’s contents from the border.

case cellLightsByBackground

If the cell is pushed in, changes the cell’s background color from gray to white.

case cellLightsByContents

If the cell is pushed in, displays the cell’s alternate image.

case cellLightsByGray

If the cell is pushed in, displays the cell’s image as darkened.

