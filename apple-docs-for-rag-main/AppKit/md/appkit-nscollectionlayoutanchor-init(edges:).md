

- AppKit
- NSCollectionLayoutAnchor
-  init(edges:) 

Initializer

# init(edges:)

Creates an anchor with the specified edges to attach to.

macOS 10.15+

``` source
@MainActor
convenience init(edges: NSDirectionalRectEdge)
```

## See Also

### Creating an anchor

convenience init(edges: NSDirectionalRectEdge, absoluteOffset: NSPoint)

Creates an anchor with the specified edges to attach to, offset by the provided absolute value.

convenience init(edges: NSDirectionalRectEdge, fractionalOffset: NSPoint)

Creates an anchor with the specified edges to attach to, offset by the provided fractional value.

