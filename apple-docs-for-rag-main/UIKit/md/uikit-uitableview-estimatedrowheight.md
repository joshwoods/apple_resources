

- UIKit
- UITableView
-  estimatedRowHeight 

Instance Property

# estimatedRowHeight

The estimated height of rows in the table view.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var estimatedRowHeight: CGFloat { get set }
```

## Mentioned in 

Estimating the height of a table’s scrolling area

## Discussion

Providing a nonnegative estimate of the height of rows can improve the performance of loading the table view. If the table contains variable height rows, it might be expensive to calculate all their heights when the table loads. Estimation allows you to defer some of the cost of geometry calculation from load time to scrolling time.

The default value is automaticDimension, which means that the table view selects an estimated height to use on your behalf. Setting the value to `0` disables estimated heights, which causes the table view to request the actual height for each cell. If your table uses self-sizing cells, the value of this property must not be `0`.

When using height estimates, the table view actively manages the contentOffset and contentSize properties inherited from its scroll view. Don’t attempt to read or modify those properties directly.

## See Also

### Related Documentation

var estimatedSectionHeaderHeight: CGFloat

The estimated height of section headers in the table view.

var estimatedSectionFooterHeight: CGFloat

The estimated height of section footers in the table view.

### Configuring cell height and layout

var rowHeight: CGFloat

The default height in points of each row in the table view.

var fillerRowHeight: CGFloat

The height for empty rows that fill the table view.

var cellLayoutMarginsFollowReadableWidth: Bool

A Boolean value that indicates whether the cell margins derive from the width of the readable content guide.

var insetsContentViewsToSafeArea: Bool

A Boolean value that indicates whether the table view adjusts the content views of its cells, headers, and footers to fit within the safe area.

