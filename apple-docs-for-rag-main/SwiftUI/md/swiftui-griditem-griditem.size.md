

- SwiftUI
- GridItem
-  GridItem.Size 

Enumeration

# GridItem.Size

The size in the minor axis of one or more rows or columns in a grid layout.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
enum Size
```

## Overview

Use a `Size` instance when you create a GridItem. The value tells a LazyHGrid how to size its rows, or a LazyVGrid how to size its columns.

## Topics

### Getting the sizes

case adaptive(minimum: CGFloat, maximum: CGFloat)

Multiple items in the space of a single flexible item.

case fixed(CGFloat)

A single item with the specified fixed size.

case flexible(minimum: CGFloat, maximum: CGFloat)

A single flexible item.

## Relationships

### Conforms To

- Sendable

## See Also

### Inspecting grid item properties

var alignment: Alignment?

The alignment to use when placing each view.

var spacing: CGFloat?

The spacing to the next item.

var size: GridItem.Size

The size of the item, which is the width of a column item or the height of a row item.

