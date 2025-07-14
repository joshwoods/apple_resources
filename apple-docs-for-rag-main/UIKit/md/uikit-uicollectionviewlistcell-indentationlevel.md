

- UIKit
- UICollectionViewListCell
-  indentationLevel 

Instance Property

# indentationLevel

The level of indentation for the cell.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var indentationLevel: Int { get set }
```

## Discussion

The indentation level sets automatically when you use a hierarchical data source, such as an NSDiffableDataSourceSectionSnapshot.

## See Also

### Customizing layout

var indentationWidth: CGFloat

The width of an indentation level.

var indentsAccessories: Bool

A Boolean value that detemines whether the cell indents accessories on the leading side.

var separatorLayoutGuide: UILayoutGuide

A guide for laying out separators in relation to the primary content in the cell.

