

- SwiftUI
- GridItem
- GridItem.Size
-  GridItem.Size.flexible(minimum:maximum:) 

Case

# GridItem.Size.flexible(minimum:maximum:)

A single flexible item.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
case flexible(
    minimum: CGFloat = 10,
    maximum: CGFloat = .infinity
)
```

## Discussion

The size of this item is the size of the grid with spacing and inflexible items removed, divided by the number of flexible items, clamped to the provided bounds.

## See Also

### Getting the sizes

case adaptive(minimum: CGFloat, maximum: CGFloat)

Multiple items in the space of a single flexible item.

case fixed(CGFloat)

A single item with the specified fixed size.

