

- AppKit
-  NSCollectionLayoutSpacing 

Class

# NSCollectionLayoutSpacing

An object that defines the space between or around items in a collection view.

macOS 10.15+

``` source
@MainActor
class NSCollectionLayoutSpacing
```

## Overview

In a collection view layout, you use a spacing object to specify both the amount of space and the way in which it’s calculated.

You can express spacing using fixed or flexible spacing.

Use *fixed spacing* to provide an exact amount of space. For example, the following code creates exactly 200 points of space between the items in the group.

- Swift
- Objective-C

```
group.interItemSpacing = .fixed(200.0)
```

```
[group setInterItemSpacing: [NSCollectionLayoutSpacing fixedSpacing:200.0]];
```

Use *flexible spacing* to provide a minimum amount of space that can grow as more space becomes available. For example, the following code creates at least 200 points of space between the items in the group. As more space becomes available, items are respaced evenly in the additional space.

- Swift
- Objective-C

```
group.interItemSpacing = .flexible(200.0)
```

```
[group setInterItemSpacing: [NSCollectionLayoutSpacing flexibleSpacing:200.0]];
```

## Topics

### Creating spacing

class func fixed(CGFloat) -> Self

Creates a space equivalent to the specified number of points.

class func flexible(CGFloat) -> Self

Creates a space equivalent to or greater than the specified number of points, depending on the available space.

### Getting the spacing value

var spacing: CGFloat

The floating-point value of the space.

### Getting the spacing type

var isFixed: Bool

A Boolean value that indicates whether the space is fixed to a specific number of points.

var isFlexible: Bool

A Boolean value that indicates whether the space is flexible.

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

class NSCollectionLayoutEdgeSpacing

An object that defines the space around the edges of items in a collection view.

protocol NSCollectionLayoutContainer

A protocol used to provide information about the size and content insets of a layout’s container.

