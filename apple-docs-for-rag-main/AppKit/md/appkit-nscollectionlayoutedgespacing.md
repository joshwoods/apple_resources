

- AppKit
-  NSCollectionLayoutEdgeSpacing 

Class

# NSCollectionLayoutEdgeSpacing

An object that defines the space around the edges of items in a collection view.

macOS 10.15+

``` source
@MainActor
class NSCollectionLayoutEdgeSpacing
```

## Overview

You use edge spacing to create additional spacing around the edges of an item to adjust the position of the item in relation to its container and other items.

The leading and trailing spaces within edge spacing differ in left-to-right versus right-to-left environments. In a left-to-right environment, the leading space is on the left, and the trailing space is on the right. In a right-to-left environment, the leading space is on the right, and the trailing space is on the left. This difference ensures that your collection view layout is built with support for right-to-left languages.

The following diagram shows the difference between adding 2 points of trailing edge spacing in a left-to-right versus a right-to-left environment.

## Topics

### Creating edge spacing

convenience init(leading: NSCollectionLayoutSpacing?, top: NSCollectionLayoutSpacing?, trailing: NSCollectionLayoutSpacing?, bottom: NSCollectionLayoutSpacing?)

Creates an edge spacing object with the specified leading, top, trailing, and bottom spacing.

### Getting the edge spacing

var leading: NSCollectionLayoutSpacing?

The leading edge spacing value.

var top: NSCollectionLayoutSpacing?

The top edge spacing value.

var trailing: NSCollectionLayoutSpacing?

The trailing edge spacing value.

var bottom: NSCollectionLayoutSpacing?

The bottom edge spacing value.

## Relationships

### Inherits From

- NSObject

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

### Size and spacing

class NSCollectionLayoutDimension

An individual dimension representing an item’s width or height in a collection view.

class NSCollectionLayoutSize

The width and the height of an item in a collection view.

class NSCollectionLayoutSpacing

An object that defines the space between or around items in a collection view.

protocol NSCollectionLayoutContainer

A protocol used to provide information about the size and content insets of a layout’s container.

