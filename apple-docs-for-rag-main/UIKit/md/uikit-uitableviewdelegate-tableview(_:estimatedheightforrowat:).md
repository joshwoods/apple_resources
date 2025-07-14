

- UIKit
- UITableViewDelegate
-  tableView(\_:estimatedHeightForRowAt:) 

Instance Method

# tableView(\_:estimatedHeightForRowAt:)

Asks the delegate for the estimated height of a row in a specified location.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    estimatedHeightForRowAt indexPath: IndexPath
) -> CGFloat
```

## Parameters 

`tableView`  

The table view requesting this information.

`indexPath`  

An index path that locates a row in `tableView`.

## Return Value

A nonnegative floating-point value that estimates the height (in points) that `row` should be. Return automaticDimension if you have no estimate.

## Mentioned in 

Estimating the height of a table’s scrolling area

## Discussion

Providing an estimate the height of rows can improve the user experience when loading the table view. If the table contains variable height rows, it might be expensive to calculate all their heights and so lead to a longer load time. Using estimation allows you to defer some of the cost of geometry calculation from load time to scrolling time.

## See Also

### Related Documentation

func tableView(UITableView, heightForRowAt: IndexPath) -> CGFloat

Asks the delegate for the height to use for a row in a specified location.

### Estimating heights for the table’s content

func tableView(UITableView, estimatedHeightForHeaderInSection: Int) -> CGFloat

Asks the delegate for the estimated height of the header of a particular section.

func tableView(UITableView, estimatedHeightForFooterInSection: Int) -> CGFloat

Asks the delegate for the estimated height of the footer of a particular section.

