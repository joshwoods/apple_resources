

- AppKit
- NSCollectionLayoutAnchor
-  init(edges:absoluteOffset:) 

Initializer

# init(edges:absoluteOffset:)

Creates an anchor with the specified edges to attach to, offset by the provided absolute value.

macOS 10.15+

``` source
@MainActor
convenience init(
    edges: NSDirectionalRectEdge,
    absoluteOffset: NSPoint
)
```

## See Also

### Creating an anchor

convenience init(edges: NSDirectionalRectEdge)

Creates an anchor with the specified edges to attach to.

convenience init(edges: NSDirectionalRectEdge, fractionalOffset: NSPoint)

Creates an anchor with the specified edges to attach to, offset by the provided fractional value.

