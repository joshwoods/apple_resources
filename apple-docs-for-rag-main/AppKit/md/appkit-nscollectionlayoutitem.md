

- AppKit
-  NSCollectionLayoutItem 

Class

# NSCollectionLayoutItem

The most basic component of a collection view’s layout.

macOS 10.15+

``` source
@MainActor
class NSCollectionLayoutItem
```

## Overview

An item is a blueprint for how to size, space, and arrange an individual piece of content in your collection view. An item represents a single view that’s rendered onscreen. Generally, an item is a cell, but items can be supplementary views like headers, footers, and other decorations.

For example, in the Photos app, an item might represent a single photo. In the App Store app, an item might be a cell displaying information about an individual app in a list of featured apps, such as the app icon, app name, tagline, and download button.

Each item specifies its own size in terms of a width dimension and a height dimension. Items can express their dimensions relative to their container, as an absolute value, or as an estimated value that might change at runtime, like in response to a change in system font size. For more information, see NSCollectionLayoutDimension.

You combine items into groups that determine how those items are arranged in relation to each other. For more information, see NSCollectionLayoutGroup.

## Topics

### Creating an item

convenience init(layoutSize: NSCollectionLayoutSize)

Creates an item of the specified size.

convenience init(layoutSize: NSCollectionLayoutSize, supplementaryItems: [NSCollectionLayoutSupplementaryItem])

Creates an item of the specified size with an array of supplementary items to attach to the item.

### Getting an item’s size

var layoutSize: NSCollectionLayoutSize

The item’s size expressed in width and height dimensions.

### Getting supplementary items

var supplementaryItems: [NSCollectionLayoutSupplementaryItem]

An array of the supplementary items attached to the item.

### Configuring spacing and insets

var edgeSpacing: NSCollectionLayoutEdgeSpacing?

The amount of space added around the boundaries of the item between other items and this item’s container.

var contentInsets: NSDirectionalEdgeInsets

The amount of space added around the content of the item to adjust its final size after its position is computed.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSCollectionLayoutDecorationItem
- NSCollectionLayoutGroup
- NSCollectionLayoutSupplementaryItem

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

class NSCollectionLayoutGroup

A container for a set of items that lays out the items along a path.

class NSCollectionLayoutSection

A container that combines a set of groups into distinct visual groupings.

