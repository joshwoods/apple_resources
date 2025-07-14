

- UIKit
- UITableViewCell
-  setSelected(\_:animated:) 

Instance Method

# setSelected(\_:animated:)

Sets the selected state of the cell, optionally animating the transition between states.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setSelected(
    _ selected: Bool,
    animated: Bool
)
```

## Parameters 

`selected`  

true to set the cell as selected, false to set it as unselected. The default is false.

`animated`  

true to animate the transition between selected states, false to make the transition immediate.

## Discussion

The selection affects the appearance of labels, image, and background. When the selected state of a cell is true, it draws the background for selected cells (Reusing cells) with its title in white.

## See Also

### Managing cell selection and highlighting

var selectionStyle: UITableViewCell.SelectionStyle

The style of selection for a cell.

enum SelectionStyle

The style of selected cells.

var isSelected: Bool

A Boolean value that indicates whether the cell is selected.

var isHighlighted: Bool

A Boolean value that indicates whether the cell is highlighted.

func setHighlighted(Bool, animated: Bool)

Sets the highlighted state of the cell, optionally animating the transition between states.

