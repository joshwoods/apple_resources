

- UIKit
- UITableView
-  automaticDimension 

Type Property

# automaticDimension

A constant representing the default value for a given dimension.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
class let automaticDimension: CGFloat
```

## Discussion

Return this value from your table view’s delegate methods when you want the table view to choose a default value for the given dimension. For example, if you return this constant from tableView(_:heightForHeaderInSection:) or tableView(_:heightForFooterInSection:), the table view uses a height that fits the value returned from tableView(_:titleForHeaderInSection:) or tableView(_:titleForFooterInSection:), if the title is not `nil`.

## See Also

### Providing header, footer, and row heights

func tableView(UITableView, heightForRowAt: IndexPath) -> CGFloat

Asks the delegate for the height to use for a row in a specified location.

func tableView(UITableView, heightForHeaderInSection: Int) -> CGFloat

Asks the delegate for the height to use for the header of a particular section.

func tableView(UITableView, heightForFooterInSection: Int) -> CGFloat

Asks the delegate for the height to use for the footer of a particular section.

