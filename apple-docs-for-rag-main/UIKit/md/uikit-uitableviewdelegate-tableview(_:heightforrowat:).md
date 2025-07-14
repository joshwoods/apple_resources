

- UIKit
- UITableViewDelegate
-  tableView(\_:heightForRowAt:) 

Instance Method

# tableView(\_:heightForRowAt:)

Asks the delegate for the height to use for a row in a specified location.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    heightForRowAt indexPath: IndexPath
) -> CGFloat
```

## Parameters 

`tableView`  

The table view requesting this information.

`indexPath`  

An index path that locates a row in `tableView`.

## Return Value

A nonnegative floating-point value that specifies the height (in points) that `row` should be.

## Mentioned in 

Configuring the cells for your table

## Discussion

Override this method when the rows of your table are not all the same height. If your rows are the same height, do not override this method; assign a value to the rowHeight property of UITableView instead. The value returned by this method takes precedence over the value in the rowHeight property.

Before it appears onscreen, the table view calls this method for the items in the visible portion of the table. As the user scrolls, the table view calls the method for items only when they move onscreen. It calls the method each time the item appears onscreen, regardless of whether it appeared onscreen previously.

## See Also

### Related Documentation

func tableView(UITableView, estimatedHeightForRowAt: IndexPath) -> CGFloat

Asks the delegate for the estimated height of a row in a specified location.

### Providing header, footer, and row heights

func tableView(UITableView, heightForHeaderInSection: Int) -> CGFloat

Asks the delegate for the height to use for the header of a particular section.

func tableView(UITableView, heightForFooterInSection: Int) -> CGFloat

Asks the delegate for the height to use for the footer of a particular section.

class let automaticDimension: CGFloat

A constant representing the default value for a given dimension.

