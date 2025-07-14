

- UIKit
- UITableView
-  UITableView.SeparatorInsetReference 

Enumeration

# UITableView.SeparatorInsetReference

Constants that indicate how to interpret the separator inset value of a table view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
enum SeparatorInsetReference
```

## Topics

### Constants

case fromCellEdges

An inset value that’s relative to the edge of the cell.

case fromAutomaticInsets

An inset value that indicates the starting position is based on the default separator insets.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var separatorInsetReference: UITableView.SeparatorInsetReference

An indicator of how to interpret the separator inset value.

