

- UIKit
- UITableViewDelegate
-  tableView(\_:estimatedHeightForHeaderInSection:) 

Instance Method

# tableView(\_:estimatedHeightForHeaderInSection:)

Asks the delegate for the estimated height of the header of a particular section.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    estimatedHeightForHeaderInSection section: Int
) -> CGFloat
```

## Parameters 

`tableView`  

The table view requesting this information.

`section`  

An index number identifying a section of `tableView` .

## Return Value

A nonnegative floating-point value that specifies the height (in points) of the header for `section`.

## Mentioned in 

Estimating the height of a table’s scrolling area

## Discussion

Providing an estimate the height of section headers can improve the user experience when loading the table view. If the table contains variable height section headers, it might be expensive to calculate all their heights and so lead to a longer load time. Using estimation allows you to defer some of the cost of geometry calculation from load time to scrolling time.

## See Also

### Related Documentation

func tableView(UITableView, heightForHeaderInSection: Int) -> CGFloat

Asks the delegate for the height to use for the header of a particular section.

### Estimating heights for the table’s content

func tableView(UITableView, estimatedHeightForRowAt: IndexPath) -> CGFloat

Asks the delegate for the estimated height of a row in a specified location.

func tableView(UITableView, estimatedHeightForFooterInSection: Int) -> CGFloat

Asks the delegate for the estimated height of the footer of a particular section.

