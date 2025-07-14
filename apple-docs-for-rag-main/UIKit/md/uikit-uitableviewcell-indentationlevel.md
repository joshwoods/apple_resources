

- UIKit
- UITableViewCell
-  indentationLevel 

Instance Property

# indentationLevel

The indentation level of the cell’s content.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var indentationLevel: Int { get set }
```

## Discussion

The default value of the property is zero (no indentation). Assigning a positive value to this property indents the cell’s content from the left edge of the cell separator. The amount of indentation is equal to the indentation level multiplied by the value in the indentationWidth property.

## See Also

### Managing content indentation

var indentationWidth: CGFloat

The width for each level of indentation of a cell’s content.

var shouldIndentWhileEditing: Bool

A Boolean value that controls whether the cell background is indented when the table view is in editing mode.

var separatorInset: UIEdgeInsets

The inset values for the separator line drawn beneath the cell.

enum SeparatorStyle

The style for cells to use as separators.

