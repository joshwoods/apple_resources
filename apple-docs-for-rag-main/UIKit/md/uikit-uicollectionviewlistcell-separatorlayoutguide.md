

- UIKit
- UICollectionViewListCell
-  separatorLayoutGuide 

Instance Property

# separatorLayoutGuide

A guide for laying out separators in relation to the primary content in the cell.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
@MainActor
var separatorLayoutGuide: UILayoutGuide { get }
```

## Discussion

This property only takes effect in a layout section that supports separators, like a section that you create using list(using:layoutEnvironment:).

The separator layout guide represents the frame of the separator, which the system uses to determine where to draw the separator at the bottom of the cell.

By default, when you apply a system-provided content configuration to a list cell, the separator automatically aligns to the primary text in the content view. For custom subviews in the cell, you need to add a constraint to this layout guide that connects it to the leading edge of the cell’s primary content.

To align the separators to your content, add constraints to the leading or trailing anchors of this layout guide.

## See Also

### Customizing layout

var indentationLevel: Int

The level of indentation for the cell.

var indentationWidth: CGFloat

The width of an indentation level.

var indentsAccessories: Bool

A Boolean value that detemines whether the cell indents accessories on the leading side.

