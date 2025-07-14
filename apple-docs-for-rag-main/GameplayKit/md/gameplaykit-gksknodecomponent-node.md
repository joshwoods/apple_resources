

- GameplayKit
- GKSKNodeComponent
-  node 

Instance Property

# node

The SpriteKit node managed by the component.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var node: SKNode { get set }
```

## Discussion

When you add this component to a GKEntity object, the component automatically sets the entity property of its SpriteKit node to point to that entity.

