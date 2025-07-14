

- AppKit
-  NSCollectionLayoutSize 

Class

# NSCollectionLayoutSize

The width and the height of an item in a collection view.

macOS 10.15+

``` source
@MainActor
class NSCollectionLayoutSize
```

## Overview

A size is a pair of dimensions (NSCollectionLayoutDimension): a width dimension and a height dimension. Every component of a collection view layout has an explicit size.

## Topics

### Creating a layout size

convenience init(widthDimension: NSCollectionLayoutDimension, heightDimension: NSCollectionLayoutDimension)

Creates a size with the specified width and height dimensions.

### Getting the width and height

var widthDimension: NSCollectionLayoutDimension

The width dimension of an item in a collection view layout.

var heightDimension: NSCollectionLayoutDimension

The height dimension of an item in a collection view layout.

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

class NSCollectionLayoutSpacing

An object that defines the space between or around items in a collection view.

class NSCollectionLayoutEdgeSpacing

An object that defines the space around the edges of items in a collection view.

protocol NSCollectionLayoutContainer

A protocol used to provide information about the size and content insets of a layout’s container.

