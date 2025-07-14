

- SceneKit
- SCNNode
-  entity 

Instance Property

# entity

The GameplayKit entity this node represents.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
weak var entity: GKEntity? { get set }
```

## Discussion

The Entity-Component architecture in the GameplayKit framework is a way to more easily manage complex object graphs in your game. For more information on this architecture, read Entities and Components in GameplayKit Programming Guide.

When you add entities (and their components) to a scene in the Xcode SceneKit Scene Editor, Xcode automatically archive those entities alongside the SceneKit scene content. Use the GKScene class to load the SceneKit scene with its associated GameplayKit objects. Each entity associated with a SceneKit node has a GKSCNNodeComponent object that manages the relationship between the node and the GKEntity object it represents.

