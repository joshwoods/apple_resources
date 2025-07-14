

- UIKit
- UITableView
-  estimatedSectionHeaderHeight 

Instance Property

# estimatedSectionHeaderHeight

The estimated height of section headers in the table view.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var estimatedSectionHeaderHeight: CGFloat { get set }
```

## Mentioned in 

Estimating the height of a table’s scrolling area

## Discussion

Providing a nonnegative estimate of the height of section headers can improve the performance of loading the table view. If the table contains variable height section headers, it might be expensive to calculate all their heights when the table loads. Estimation allows you to defer some of the cost of geometry calculation from load time to scrolling time.

The default value is automaticDimension, which means that the table view selects an estimated height to use on your behalf. Setting the value to `0` disables estimated heights, which causes the table view to request the actual height for each header. If your table uses self-sizing headers, the value of this property must not be `0`.

When using height estimates, the table view actively manages the contentOffset and contentSize properties inherited from its scroll view. Don’t attempt to read or modify those properties directly.

## See Also

### Related Documentation

var estimatedRowHeight: CGFloat

The estimated height of rows in the table view.

### Configuring header and footer appearance

var sectionHeaderHeight: CGFloat

The height of section headers in the table view.

var sectionFooterHeight: CGFloat

The height of section footers in the table view.

var estimatedSectionFooterHeight: CGFloat

The estimated height of section footers in the table view.

var sectionHeaderTopPadding: CGFloat

The amount of padding above each section header.

