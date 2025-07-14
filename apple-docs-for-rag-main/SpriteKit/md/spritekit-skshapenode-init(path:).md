

- SpriteKit
- SKShapeNode
-  init(path:) 

Initializer

# init(path:)

Creates a shape node from a Core Graphics path.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(path: CGPath)
```

**watchOS**

``` source
convenience init(path: CGPath)
```

## Parameters 

`path`  

The Core Graphics path to use. The path is relative to the node’s origin.

## Return Value

A new shape node.

## See Also

### Creating a Shape from a Path

convenience init(path: CGPath, centered: Bool)

Creates a shape node from a Core Graphics path, centered around its position.

var path: CGPath?

The path that defines the shape.

