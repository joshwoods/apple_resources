

- UIKit
- UITableViewCell
-  shouldIndentWhileEditing 

Instance Property

# shouldIndentWhileEditing

A Boolean value that controls whether the cell background is indented when the table view is in editing mode.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var shouldIndentWhileEditing: Bool { get set }
```

## Discussion

The default value is true. This property is unrelated to indentationLevel. The delegate can override this value in tableView(_:shouldIndentWhileEditingRowAt:). This property has an effect only on table views created in the grouped style (UITableView.Style.grouped); it has no effect on UITableView.Style.plain table views.

## See Also

### Managing content indentation

var indentationLevel: Int

The indentation level of the cell’s content.

var indentationWidth: CGFloat

The width for each level of indentation of a cell’s content.

var separatorInset: UIEdgeInsets

The inset values for the separator line drawn beneath the cell.

enum SeparatorStyle

The style for cells to use as separators.

