

- UIKit
- UITableViewCell
-  setHighlighted(\_:animated:) 

Instance Method

# setHighlighted(\_:animated:)

Sets the highlighted state of the cell, optionally animating the transition between states.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setHighlighted(
    _ highlighted: Bool,
    animated: Bool
)
```

## Parameters 

`highlighted`  

true to set the cell as highlighted, false to set it as unhighlighted. The default is false.

`animated`  

true to animate the transition between highlighted states, false to make the transition immediate.

## Discussion

Highlights or unhighlights the cell, animating the transition between regular and highlighted state if `animated` is YES. Highlighting affects the appearance of the cell’s labels, image, and background.

Note that for highlighting to work properly, you must fetch the cell’s label (or labels) using the textLabel (and detailTextLabel properties and set the label’s highlightedTextColor property; for images, get the cell’s image using the imageView property and set the UIImageView object’s `highlightedImage` property.

A custom table cell may override this method to make any transitory appearance changes.

## See Also

### Managing cell selection and highlighting

var selectionStyle: UITableViewCell.SelectionStyle

The style of selection for a cell.

enum SelectionStyle

The style of selected cells.

var isSelected: Bool

A Boolean value that indicates whether the cell is selected.

func setSelected(Bool, animated: Bool)

Sets the selected state of the cell, optionally animating the transition between states.

var isHighlighted: Bool

A Boolean value that indicates whether the cell is highlighted.

