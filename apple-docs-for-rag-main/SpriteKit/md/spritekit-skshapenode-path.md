

- SpriteKit
- SKShapeNode
-  path 

Instance Property

# path

The path that defines the shape.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var path: CGPath? { get set }
```

**watchOS**

``` source
var path: CGPath? { get set }
```

## Mentioned in 

Getting Started with Shape Nodes

## Discussion

The path is defined in the node’s coordinate space.

## See Also

### Creating a Shape from a Path

convenience init(path: CGPath)

Creates a shape node from a Core Graphics path.

convenience init(path: CGPath, centered: Bool)

Creates a shape node from a Core Graphics path, centered around its position.

