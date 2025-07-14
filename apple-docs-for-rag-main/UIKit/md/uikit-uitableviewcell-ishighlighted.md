

- UIKit
- UITableViewCell
-  isHighlighted 

Instance Property

# isHighlighted

A Boolean value that indicates whether the cell is highlighted.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isHighlighted: Bool { get set }
```

## Discussion

The highlighting affects the appearance of labels, image, and background. When the highlighted state of a cell is set to true, labels are drawn in their highlighted text color (default is white). The default value is false. If you set the highlighted state to true through this property, the transition to the new state appearance is not animated. For animated highlighted-state transitions, see the setHighlighted(_:animated:) method.

Note that for highlighting to work properly, you must fetch the cell’s labels using the textLabel and detailTextLabel properties and set each label’s highlightedTextColor property; for images, get the cell’s image using the imageView property and set the UIImageView object’s `highlightedImage` property.

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

func setHighlighted(Bool, animated: Bool)

Sets the highlighted state of the cell, optionally animating the transition between states.

