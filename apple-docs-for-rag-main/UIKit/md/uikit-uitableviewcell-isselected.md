

- UIKit
- UITableViewCell
-  isSelected 

Instance Property

# isSelected

A Boolean value that indicates whether the cell is selected.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isSelected: Bool { get set }
```

## Discussion

The selection affects the appearance of labels, image, and background. When the selected state of a cell is set to true, it draws the background for selected cells with its title in white. The default value is false. If you set the selection state to true through this property, the transition to the new state appearance is not animated. For animated selected-state transitions, see the setSelected(_:animated:) method.

## See Also

### Managing cell selection and highlighting

var selectionStyle: UITableViewCell.SelectionStyle

The style of selection for a cell.

enum SelectionStyle

The style of selected cells.

func setSelected(Bool, animated: Bool)

Sets the selected state of the cell, optionally animating the transition between states.

var isHighlighted: Bool

A Boolean value that indicates whether the cell is highlighted.

func setHighlighted(Bool, animated: Bool)

Sets the highlighted state of the cell, optionally animating the transition between states.

