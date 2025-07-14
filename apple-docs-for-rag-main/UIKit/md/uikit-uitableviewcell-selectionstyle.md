

- UIKit
- UITableViewCell
-  selectionStyle 

Instance Property

# selectionStyle

The style of selection for a cell.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var selectionStyle: UITableViewCell.SelectionStyle { get set }
```

## Discussion

The selection style is a backgroundView constant that determines the color of a cell when it’s selected. The default value is UITableViewCell.SelectionStyle.default. See UITableViewCell.SelectionStyle for a description of valid constants.

## See Also

### Managing cell selection and highlighting

enum SelectionStyle

The style of selected cells.

var isSelected: Bool

A Boolean value that indicates whether the cell is selected.

func setSelected(Bool, animated: Bool)

Sets the selected state of the cell, optionally animating the transition between states.

var isHighlighted: Bool

A Boolean value that indicates whether the cell is highlighted.

func setHighlighted(Bool, animated: Bool)

Sets the highlighted state of the cell, optionally animating the transition between states.

