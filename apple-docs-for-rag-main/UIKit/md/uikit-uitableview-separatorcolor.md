

- UIKit
- UITableView
-  separatorColor 

Instance Property

# separatorColor

The color of separator rows in the table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var separatorColor: UIColor? { get set }
```

## Discussion

The default color is gray.

## See Also

### Customizing the separator appearance

var separatorStyle: UITableViewCell.SeparatorStyle

The style for table cells to use as separators.

enum SeparatorStyle

The style for cells to use as separators.

var separatorEffect: UIVisualEffect?

The effect to apply to table separators.

var separatorInset: UIEdgeInsets

The default inset of cell separators.

var separatorInsetReference: UITableView.SeparatorInsetReference

An indicator of how to interpret the separator inset value.

enum SeparatorInsetReference

Constants that indicate how to interpret the separator inset value of a table view.

