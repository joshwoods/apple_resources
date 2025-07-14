

- UIKit
- NSCollectionLayoutAnchor
-  init(edges:absoluteOffset:) 

Initializer

# init(edges:absoluteOffset:)

Creates an anchor with the specified edges to attach to, offset by the provided absolute value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
convenience init(
    edges: NSDirectionalRectEdge,
    absoluteOffset: CGPoint
)
```

## See Also

### Creating an anchor

convenience init(edges: NSDirectionalRectEdge)

Creates an anchor with the specified edges to attach to.

convenience init(edges: NSDirectionalRectEdge, fractionalOffset: CGPoint)

Creates an anchor with the specified edges to attach to, offset by the provided fractional value.

