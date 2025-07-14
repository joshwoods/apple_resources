

- UIKit
- UITableView
-  sectionFooterHeight 

Instance Property

# sectionFooterHeight

The height of section footers in the table view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var sectionFooterHeight: CGFloat { get set }
```

## Mentioned in 

Adding headers and footers to table sections

## Discussion

The default value is automaticDimension. If the delegate doesn’t implement tableView(_:heightForFooterInSection:), the table view calculates the height automatically. To override automatic height calculation, set this property to a positive value.

## See Also

### Related Documentation

var tableFooterView: UIView?

The view that displays below the table’s content.

### Configuring header and footer appearance

var sectionHeaderHeight: CGFloat

The height of section headers in the table view.

var estimatedSectionHeaderHeight: CGFloat

The estimated height of section headers in the table view.

var estimatedSectionFooterHeight: CGFloat

The estimated height of section footers in the table view.

var sectionHeaderTopPadding: CGFloat

The amount of padding above each section header.

