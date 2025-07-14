

- UIKit
- UITableViewDelegate
-  tableView(\_:heightForFooterInSection:) 

Instance Method

# tableView(\_:heightForFooterInSection:)

Asks the delegate for the height to use for the footer of a particular section.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    heightForFooterInSection section: Int
) -> CGFloat
```

## Parameters 

`tableView`  

The table view requesting this information.

`section`  

An index number identifying a section of `tableView` .

## Return Value

A nonnegative floating-point value that specifies the height (in points) of the footer for `section`.

## Mentioned in 

Adding headers and footers to table sections

## Discussion

Use this method to specify the height of custom header views returned by your tableView(_:viewForFooterInSection:) method.

## See Also

### Related Documentation

func tableView(UITableView, viewForFooterInSection: Int) -> UIView?

Asks the delegate for a view to display in the footer of the specified section of the table view.

func tableView(UITableView, estimatedHeightForFooterInSection: Int) -> CGFloat

Asks the delegate for the estimated height of the footer of a particular section.

### Providing header, footer, and row heights

func tableView(UITableView, heightForRowAt: IndexPath) -> CGFloat

Asks the delegate for the height to use for a row in a specified location.

func tableView(UITableView, heightForHeaderInSection: Int) -> CGFloat

Asks the delegate for the height to use for the header of a particular section.

class let automaticDimension: CGFloat

A constant representing the default value for a given dimension.

