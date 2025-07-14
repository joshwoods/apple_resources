

- UIKit
- UITableView
-  backgroundView 

Instance Property

# backgroundView

The background view of the table view.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var backgroundView: UIView? { get set }
```

## Discussion

Assign a background view to change the color behind your table’s sections and rows. The default value of this property is `nil`.

When you assign a view to this property, the table view automatically resizes that view to match its own bounds. Your background view appears behind all cells, header views, and footer views and doesn’t scroll with the rest of the table’s content.

## See Also

### Configuring the table’s appearance

var style: UITableView.Style

The style of the table view.

enum Style

Constants for the table view styles.

var tableHeaderView: UIView?

The view that displays above the table’s content.

var tableFooterView: UIView?

The view that displays below the table’s content.

