

- SpriteKit
- SKShapeNode
-  init(path:centered:) 

Initializer

# init(path:centered:)

Creates a shape node from a Core Graphics path, centered around its position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(
    path: CGPath,
    centered: Bool
)
```

**watchOS**

``` source
convenience init(
    path: CGPath,
    centered: Bool
)
```

## Parameters 

`path`  

The Core Graphics path to use.

`centered`  

If true, the path is translated so that the center of the path’s bounding box is at the node’s origin; otherwise the path is relative to the node’s origin.

## Return Value

A new shape node.

## See Also

### Creating a Shape from a Path

convenience init(path: CGPath)

Creates a shape node from a Core Graphics path.

var path: CGPath?

The path that defines the shape.

