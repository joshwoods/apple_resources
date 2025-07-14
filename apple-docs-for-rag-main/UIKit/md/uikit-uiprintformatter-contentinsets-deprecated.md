

- UIKit
- UIPrintFormatter
-  contentInsets Deprecated

Instance Property

# contentInsets

The distances the edges of content are inset from the printing rectangle.

iOS 4.2–10.0DeprecatediPadOS 4.2–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var contentInsets: UIEdgeInsets { get set }
```

## Discussion

This property adjusts the margins for content printed by the formatter. The printing rectangle defines the area the printer is capable of printing in; each inset is an inward distance, in points, from a side of the printing area. The top inset is used only on the first page that the formatter draws. The bottom inset is not used. You can use the init(top:left:bottom:right:) macro to create a UIEdgeInsets structure.

The default value of this property is zero.

## See Also

### Laying out the content

var perPageContentInsets: UIEdgeInsets

The margins for each printed page.

var maximumContentHeight: CGFloat

The maximum height of the content area.

var maximumContentWidth: CGFloat

The maximum width of the content area.

