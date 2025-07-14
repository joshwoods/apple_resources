

- UIKit
- UITableView
-  insetsContentViewsToSafeArea 

Instance Property

# insetsContentViewsToSafeArea

A Boolean value that indicates whether the table view adjusts the content views of its cells, headers, and footers to fit within the safe area.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var insetsContentViewsToSafeArea: Bool { get set }
```

## Discussion

When the value of this property is true (the default), the table view adjusts the insets of the content view within each of its cells, headers, and footers on the leading and trailing sides to make the content fit within the safe area. The safe area ensures that the content within the table view isn’t obscured by other views, or by the edges of the device.

When the value of this property is false, the table view doesn’t adjust the insets of the content view within each of its cells, headers, and footers to account for the safe area. In this case, the content views extend to the bounds of their respective superviews, which may cause the content to be obscured.

## See Also

### Related Documentation

var safeAreaInsets: UIEdgeInsets

The insets that you use to determine the safe area for this view.

### Configuring cell height and layout

var rowHeight: CGFloat

The default height in points of each row in the table view.

var estimatedRowHeight: CGFloat

The estimated height of rows in the table view.

var fillerRowHeight: CGFloat

The height for empty rows that fill the table view.

var cellLayoutMarginsFollowReadableWidth: Bool

A Boolean value that indicates whether the cell margins derive from the width of the readable content guide.

