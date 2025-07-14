

- UIKit
- UITableView
-  sectionHeaderHeight 

Instance Property

# sectionHeaderHeight

The height of section headers in the table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var sectionHeaderHeight: CGFloat { get set }
```

## Mentioned in 

Adding headers and footers to table sections

## Discussion

The default value is automaticDimension. If the delegate doesn’t implement tableView(_:heightForHeaderInSection:), the table view calculates the height automatically. To override automatic height calculation, set this property to a positive value.

## See Also

### Related Documentation

var tableHeaderView: UIView?

The view that displays above the table’s content.

### Configuring header and footer appearance

var sectionFooterHeight: CGFloat

The height of section footers in the table view.

var estimatedSectionHeaderHeight: CGFloat

The estimated height of section headers in the table view.

var estimatedSectionFooterHeight: CGFloat

The estimated height of section footers in the table view.

var sectionHeaderTopPadding: CGFloat

The amount of padding above each section header.

