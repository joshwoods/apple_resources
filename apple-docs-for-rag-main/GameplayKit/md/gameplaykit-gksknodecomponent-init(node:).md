

- GameplayKit
- GKSKNodeComponent
-  init(node:) 

Initializer

# init(node:)

Initializes a component to manage the specified SpriteKit node.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
init(node: SKNode)
```

## Parameters 

`node`  

The SpriteKit node to be managed by the component.

## Return Value

A new SpriteKit component.

## Discussion

When you add this component to a GKEntity object, the component automatically sets the entity property of its SpriteKit node to point to that entity.

