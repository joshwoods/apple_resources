

- SwiftUI
- GridItem
- GridItem.Size
-  GridItem.Size.adaptive(minimum:maximum:) 

Case

# GridItem.Size.adaptive(minimum:maximum:)

Multiple items in the space of a single flexible item.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
case adaptive(
    minimum: CGFloat,
    maximum: CGFloat = .infinity
)
```

## Discussion

This size case places one or more items into the space assigned to a single `flexible` item, using the provided bounds and spacing to decide exactly how many items fit. This approach prefers to insert as many items of the `minimum` size as possible but lets them increase to the `maximum` size.

## See Also

### Getting the sizes

case fixed(CGFloat)

A single item with the specified fixed size.

case flexible(minimum: CGFloat, maximum: CGFloat)

A single flexible item.

