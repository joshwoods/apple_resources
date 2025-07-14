

- UIKit
- UITableView
-  separatorStyle 

Instance Property

# separatorStyle

The style for table cells to use as separators.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var separatorStyle: UITableViewCell.SeparatorStyle { get set }
```

## Discussion

The value of this property is one of the separator-style constants described in UITableViewCell. `UITableView` uses this property to set the separator style on the cell returned from the delegate in tableView(_:cellForRowAt:).

## See Also

### Customizing the separator appearance

enum SeparatorStyle

The style for cells to use as separators.

var separatorColor: UIColor?

The color of separator rows in the table view.

var separatorEffect: UIVisualEffect?

The effect to apply to table separators.

var separatorInset: UIEdgeInsets

The default inset of cell separators.

var separatorInsetReference: UITableView.SeparatorInsetReference

An indicator of how to interpret the separator inset value.

enum SeparatorInsetReference

Constants that indicate how to interpret the separator inset value of a table view.

