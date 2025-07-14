

- AppKit
-  NSCollectionLayoutGroup 

Class

# NSCollectionLayoutGroup

A container for a set of items that lays out the items along a path.

macOS 10.15+

``` source
@MainActor
class NSCollectionLayoutGroup
```

## Overview

Groups determine how the items in a collection view lay out in relation to each other. A group might lay out its items in a horizontal row, a vertical column, or a custom arrangement. A group determines the rules for how items are rendered in relation to each other, but in itself doesn’t render any content.

For example, in the Photos app, a group of items is a row of photos. In the App Store app, a group might be a single column of cells (items) arranged in a vertical column.

Each group specifies its own size in terms of a width dimension and a height dimension. Groups can express their dimensions relative to their container, as an absolute value, or as an estimated value that might change at runtime, like in response to a change in system font size. For more information, see NSCollectionLayoutDimension.

Because a group is a subclass of NSCollectionLayoutItem, it behaves like an item. You can combine a group with other items and groups into more complex layouts.

After you configure a group, you must initialize a section (NSCollectionLayoutSection) of your collection view layout with that group.

## Topics

### Creating a horizontal group

class func horizontal(layoutSize: NSCollectionLayoutSize, subitems: [NSCollectionLayoutItem]) -> Self

Creates a group of the specified size, containing an array of items arranged in a horizontal line.

class func horizontal(layoutSize: NSCollectionLayoutSize, subitem: NSCollectionLayoutItem, count: Int) -> Self

Creates a group of the specified size, containing an array of equally sized items arranged in a horizontal line up to the number specified by count.

### Creating a vertical group

class func vertical(layoutSize: NSCollectionLayoutSize, subitems: [NSCollectionLayoutItem]) -> Self

Creates a group of the specified size, containing an array of items arranged in a vertical line.

class func vertical(layoutSize: NSCollectionLayoutSize, subitem: NSCollectionLayoutItem, count: Int) -> Self

Creates a group of the specified size, containing an array of equally sized items arranged in a vertical line up to the number specified by count.

### Creating a custom group

class func custom(layoutSize: NSCollectionLayoutSize, itemProvider: NSCollectionLayoutGroupCustomItemProvider) -> Self

Creates a group of the specified size, with an item provider that creates a custom arrangement for those items.

### Getting the group’s items

var subitems: [NSCollectionLayoutItem]

An array of the items contained in the group.

var supplementaryItems: [NSCollectionLayoutSupplementaryItem]

An array of the supplementary items that are anchored to the group.

### Configuring group spacing

var interItemSpacing: NSCollectionLayoutSpacing?

The amount of space between the items in the group.

### Debugging group layout

func visualDescription() -> String

Returns a string with an ASCII representation of the group.

## Relationships

### Inherits From

- NSCollectionLayoutItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Components

class NSCollectionLayoutItem

The most basic component of a collection view’s layout.

class NSCollectionLayoutSection

A container that combines a set of groups into distinct visual groupings.

