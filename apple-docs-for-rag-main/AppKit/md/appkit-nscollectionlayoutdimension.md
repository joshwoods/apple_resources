

- AppKit
-  NSCollectionLayoutDimension 

Class

# NSCollectionLayoutDimension

An individual dimension representing an item’s width or height in a collection view.

macOS 10.15+

``` source
@MainActor
class NSCollectionLayoutDimension
```

## Overview

Each item in a collection view has an explicit width dimension and height dimension, which combine to define the item’s size (NSCollectionLayoutSize).

You can express an item’s dimensions using an absolute, estimated, or fractional value.

Use an *absolute value* to specify exact dimensions, like a 44 x 44 point square:

- Swift
- Objective-C

```
let absoluteSize = NSCollectionLayoutSize(widthDimension: .absolute(44),
                                         heightDimension: .absolute(44))
```

```
NSCollectionLayoutSize *absoluteSize = [NSCollectionLayoutSize sizeWithWidthDimension:[NSCollectionLayoutDimension absoluteDimension:44.0] heightDimension:[NSCollectionLayoutDimension absoluteDimension:44.0]];
```

Use an *estimated value* if the size of your content might change at runtime, such as when data is loaded or in response to a change in system font size. You provide an initial estimated size and the system computes the actual value later.

- Swift
- Objective-C

```
let estimatedSize = NSCollectionLayoutSize(widthDimension: .estimated(200),
                                          heightDimension: .estimated(100))
```

```
NSCollectionLayoutSize *estimatedSize = [NSCollectionLayoutSize sizeWithWidthDimension:[NSCollectionLayoutDimension estimatedDimension:200.0] heightDimension:[NSCollectionLayoutDimension estimatedDimension:100.0]];
```

Use a *fractional value* to define a value that’s relative to a dimension of the item’s container. This option simplifies specifying aspect ratios. For example, the following item has a width and a height that are both equal to 20% of its container’s width, creating a square that grows and shrinks as the size of its container changes.

- Swift
- Objective-C

```
let fractionalSize = NSCollectionLayoutSize(widthDimension: .fractionalWidth(0.2),
                                           heightDimension: .fractionalWidth(0.2))
```

```
NSCollectionLayoutSize *fractionalSize = [NSCollectionLayoutSize sizeWithWidthDimension:[NSCollectionLayoutDimension fractionalWidthDimension:0.2] heightDimension:[NSCollectionLayoutDimension fractionalWidthDimension:0.2]];
```

## Topics

### Creating a dimension

class func absolute(CGFloat) -> Self

Creates a dimension with an absolute point value.

class func estimated(CGFloat) -> Self

Creates a dimension with an estimated point value.

class func fractionalHeight(CGFloat) -> Self

Creates a dimension that is computed as a fraction of the height of the containing group.

class func fractionalWidth(CGFloat) -> Self

Creates a dimension that is computed as a fraction of the width of the containing group.

### Getting the dimension value

var dimension: CGFloat

The floating-point value of the dimension.

### Getting the dimension type

var isAbsolute: Bool

A Boolean value that indicates whether the dimension is expressed as an absolute value.

var isEstimated: Bool

A Boolean value that indicates whether the dimension is expressed as an estimated value.

var isFractionalHeight: Bool

A Boolean value that indicates whether the dimension is expressed as a fraction of its container’s height.

var isFractionalWidth: Bool

A Boolean value that indicates whether the dimension is expressed as a fraction of its container’s width.

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

class NSCollectionLayoutSize

The width and the height of an item in a collection view.

class NSCollectionLayoutSpacing

An object that defines the space between or around items in a collection view.

class NSCollectionLayoutEdgeSpacing

An object that defines the space around the edges of items in a collection view.

protocol NSCollectionLayoutContainer

A protocol used to provide information about the size and content insets of a layout’s container.

