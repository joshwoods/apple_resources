

- UIKit
- UIPrintFormatter
-  maximumContentWidth 

Instance Property

# maximumContentWidth

The maximum width of the content area.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var maximumContentWidth: CGFloat { get set }
```

## Discussion

`UIPrintFormatter` uses this value to determine the maximum width of the content rectangle. It compares the value of this property with the printing rectangle’s width minus the left and right inset values and uses the lower of the two. The default value of this property is the maximum float value.

## See Also

### Laying out the content

var perPageContentInsets: UIEdgeInsets

The margins for each printed page.

var maximumContentHeight: CGFloat

The maximum height of the content area.

var contentInsets: UIEdgeInsets

The distances the edges of content are inset from the printing rectangle.

Deprecated

