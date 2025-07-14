

- UIKit
- UITableView
- UITableView.SeparatorInsetReference
-  UITableView.SeparatorInsetReference.fromAutomaticInsets 

Case

# UITableView.SeparatorInsetReference.fromAutomaticInsets

An inset value that indicates the starting position is based on the default separator insets.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
case fromAutomaticInsets
```

## Discussion

When using this style, the values in the separatorInset property are interpreted as offsets from the default insets provided by the table view. The table view normally uses its layout margins as the default cell inset value. However, these insets may be modified by other factors, such as the when the cellLayoutMarginsFollowReadableWidth property is set to true.

## See Also

### Constants

case fromCellEdges

An inset value that’s relative to the edge of the cell.

