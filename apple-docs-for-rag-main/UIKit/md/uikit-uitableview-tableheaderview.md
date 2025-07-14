

- UIKit
- UITableView
-  tableHeaderView 

Instance Property

# tableHeaderView

The view that displays above the table’s content.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var tableHeaderView: UIView? { get set }
```

## Mentioned in 

Adding headers and footers to table sections

## Discussion

Use this property to specify a header view for your entire table. The header view is the first item to appear in the table’s view’s scrolling content, and it’s separate from the header views you add to individual sections. The default value of this property is `nil`.

When assigning a view to this property, set the height of that view to a nonzero value. The table view respects only the height of your view’s frame rectangle; it adjusts the width of your header view automatically to match the table view’s width.

## See Also

### Related Documentation

var sectionHeaderHeight: CGFloat

The height of section headers in the table view.

### Configuring the table’s appearance

var style: UITableView.Style

The style of the table view.

enum Style

Constants for the table view styles.

var tableFooterView: UIView?

The view that displays below the table’s content.

var backgroundView: UIView?

The background view of the table view.

