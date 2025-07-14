

- UIKit
- UIPrintFormatter
-  perPageContentInsets 

Instance Property

# perPageContentInsets

The margins for each printed page.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var perPageContentInsets: UIEdgeInsets { get set }
```

## Discussion

This property specifies the margins to apply to each printed page. All margins are respected, so the top inset value represents the top margin of every page, the left inset value represents the left margin of every page, and so on. If the per-page insets are smaller than the printable area of the page, or smaller than the printable area after the values in the contentInsets property are applied, the value in this property is effectively ignored.

The default value of this property is zero.

## See Also

### Laying out the content

var maximumContentHeight: CGFloat

The maximum height of the content area.

var maximumContentWidth: CGFloat

The maximum width of the content area.

var contentInsets: UIEdgeInsets

The distances the edges of content are inset from the printing rectangle.

Deprecated

