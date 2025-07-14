

- UIKit
- UITableView
-  separatorInsetReference 

Instance Property

# separatorInsetReference

An indicator of how to interpret the separator inset value.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var separatorInsetReference: UITableView.SeparatorInsetReference { get set }
```

## Discussion

Use the value of this property to determine how the value in the separatorInset property is interpreted for cells. The default value of this property is UITableView.SeparatorInsetReference.fromCellEdges.

## See Also

### Customizing the separator appearance

var separatorStyle: UITableViewCell.SeparatorStyle

The style for table cells to use as separators.

enum SeparatorStyle

The style for cells to use as separators.

var separatorColor: UIColor?

The color of separator rows in the table view.

var separatorEffect: UIVisualEffect?

The effect to apply to table separators.

var separatorInset: UIEdgeInsets

The default inset of cell separators.

enum SeparatorInsetReference

Constants that indicate how to interpret the separator inset value of a table view.

