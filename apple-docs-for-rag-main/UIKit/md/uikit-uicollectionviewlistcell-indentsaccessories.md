

- UIKit
- UICollectionViewListCell
-  indentsAccessories 

Instance Property

# indentsAccessories

A Boolean value that detemines whether the cell indents accessories on the leading side.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var indentsAccessories: Bool { get set }
```

## Discussion

If the value is false, the cell indents the content view only.

The default value of this property is true.

## See Also

### Customizing layout

var indentationLevel: Int

The level of indentation for the cell.

var indentationWidth: CGFloat

The width of an indentation level.

var separatorLayoutGuide: UILayoutGuide

A guide for laying out separators in relation to the primary content in the cell.

