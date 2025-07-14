

- UIKit
-  NSCollectionLayoutAnchor 

Class

# NSCollectionLayoutAnchor

An object that defines how to attach a supplementary item to an item in a collection view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class NSCollectionLayoutAnchor
```

## Overview

You use an anchor to attach a supplementary item to a specific item. An anchor contains information about where on the item your supplementary item is attached, including:

- An edge or set of edges. You can attach a supplementary item to a single edge, or to a corner by specifying two adjacent edges.

- An offset from the item. By default, the supplementary item is anchored within the specified edges of the item it’s attached to. You can change this location by providing a custom offset when you create an anchor.

### Edges

The leading and trailing edges for anchors differ in left-to-right versus right-to-left environments. In a left-to-right environment, the leading edge is on the left, and the trailing edge is on the right. In a right-to-left environment, the leading edge is on the right, and the trailing edge is on the left. This difference ensures that your collection view layout is built with support for right-to-left languages.

The following diagram shows anchor placement for the specified edges in a left-to-right environment.

### Offset

You can express anchor offset in these ways:

- Absolute value. The offset is calculated as a point value. For example, an absolute x offset of `30.0` means that the origin of the supplementary item is offset by 30 points in the positive x direction.

- Fractional value. The offset is calculated as a fraction of the supplementary item’s dimensions. For example, a fractional x offset of `0.3` means that the origin of the supplementary item is offset by 30% of the supplementary item’s width in the positive x direction.

The following code creates a basic badge and attaches it to an item’s top trailing corner.

- Swift
- Objective-C

```
let itemSize = NSCollectionLayoutSize(widthDimension: .absolute(44),
                                     heightDimension: .absolute(44))

let badgeAnchor = NSCollectionLayoutAnchor(edges: [.top, .trailing],
                                fractionalOffset: CGPoint(x: 0.3, y: -0.3))

let badgeSize = NSCollectionLayoutSize(widthDimension: .absolute(20),
                                      heightDimension: .absolute(20))

let badge = NSCollectionLayoutSupplementaryItem(layoutSize: badgeSize,
                                               elementKind: "badge",
                                           containerAnchor: badgeAnchor)

let item = NSCollectionLayoutItem(layoutSize: itemSize,
                          supplementaryItems: [badge])

```

```
NSCollectionLayoutSize *itemSize = [NSCollectionLayoutSize sizeWithWidthDimension:[NSCollectionLayoutDimension absoluteDimension:44.0] heightDimension:[NSCollectionLayoutDimension absoluteDimension:44.0]];

NSCollectionLayoutAnchor *badgeAnchor = [NSCollectionLayoutAnchor layoutAnchorWithEdges: NSDirectionalRectEdgeTop|NSDirectionalRectEdgeTrailing fractionalOffset:CGPointMake(0.3, -0.3)];

NSCollectionLayoutSize *badgeSize = [NSCollectionLayoutSize sizeWithWidthDimension:[NSCollectionLayoutDimension absoluteDimension:20.0] heightDimension:[NSCollectionLayoutDimension absoluteDimension:20.0]];

NSCollectionLayoutSupplementaryItem *badge = [NSCollectionLayoutSupplementaryItem supplementaryItemWithLayoutSize:badgeSize elementKind:ELEMENT_KIND_BADGE containerAnchor:badgeAnchor];

NSCollectionLayoutItem *item = [NSCollectionLayoutItem itemWithLayoutSize:itemSize supplementaryItems:@[badge]];
```

## Topics

### Creating an anchor

convenience init(edges: NSDirectionalRectEdge)

Creates an anchor with the specified edges to attach to.

convenience init(edges: NSDirectionalRectEdge, absoluteOffset: CGPoint)

Creates an anchor with the specified edges to attach to, offset by the provided absolute value.

convenience init(edges: NSDirectionalRectEdge, fractionalOffset: CGPoint)

Creates an anchor with the specified edges to attach to, offset by the provided fractional value.

### Getting the edges

var edges: NSDirectionalRectEdge

The edges of the item an anchor is attached to.

### Getting the offset

var offset: CGPoint

The floating-point value of the anchor’s offset from the item it’s attached to.

var isAbsoluteOffset: Bool

A Boolean value that indicates whether the anchor’s offset is expressed as an absolute value.

var isFractionalOffset: Bool

A Boolean value that indicates whether the anchor’s offset is expressed as a fraction of its supplementary item’s dimension.

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

### Appearance

class NSCollectionLayoutSupplementaryItem

An object used to add an extra visual decoration to an item in a collection view.

class NSCollectionLayoutBoundarySupplementaryItem

An object used to add headers or footers to a collection view.

class NSCollectionLayoutDecorationItem

An object used to add a background to a section of a collection view.

