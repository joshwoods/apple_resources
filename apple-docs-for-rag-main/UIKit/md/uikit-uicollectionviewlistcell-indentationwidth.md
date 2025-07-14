

- UIKit
- UICollectionViewListCell
-  indentationWidth 

Instance Property

# indentationWidth

The width of an indentation level.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var indentationWidth: CGFloat { get set }
```

## Discussion

The overall indentation is the product of indentationWidth and indentationLevel.

## See Also

### Customizing layout

var indentationLevel: Int

The level of indentation for the cell.

var indentsAccessories: Bool

A Boolean value that detemines whether the cell indents accessories on the leading side.

var separatorLayoutGuide: UILayoutGuide

A guide for laying out separators in relation to the primary content in the cell.

