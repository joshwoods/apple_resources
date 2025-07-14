

- UIKit
- NSCollectionLayoutAnchor
-  init(edges:fractionalOffset:) 

Initializer

# init(edges:fractionalOffset:)

Creates an anchor with the specified edges to attach to, offset by the provided fractional value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
convenience init(
    edges: NSDirectionalRectEdge,
    fractionalOffset: CGPoint
)
```

## See Also

### Creating an anchor

convenience init(edges: NSDirectionalRectEdge)

Creates an anchor with the specified edges to attach to.

convenience init(edges: NSDirectionalRectEdge, absoluteOffset: CGPoint)

Creates an anchor with the specified edges to attach to, offset by the provided absolute value.

