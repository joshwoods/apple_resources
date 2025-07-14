

- UIKit
- UITableViewDelegate
-  tableView(\_:heightForHeaderInSection:) 

Instance Method

# tableView(\_:heightForHeaderInSection:)

Asks the delegate for the height to use for the header of a particular section.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func tableView(
    _ tableView: UITableView,
    heightForHeaderInSection section: Int
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

Adding headers and footers to table sections

## Discussion

Use this method to specify the height of custom header views returned by your tableView(_:viewForHeaderInSection:) method.

## See Also

### Related Documentation

func tableView(UITableView, estimatedHeightForHeaderInSection: Int) -> CGFloat

Asks the delegate for the estimated height of the header of a particular section.

func tableView(UITableView, viewForHeaderInSection: Int) -> UIView?

Asks the delegate for a view to display in the header of the specified section of the table view.

### Providing header, footer, and row heights

func tableView(UITableView, heightForRowAt: IndexPath) -> CGFloat

Asks the delegate for the height to use for a row in a specified location.

func tableView(UITableView, heightForFooterInSection: Int) -> CGFloat

Asks the delegate for the height to use for the footer of a particular section.

class let automaticDimension: CGFloat

A constant representing the default value for a given dimension.

