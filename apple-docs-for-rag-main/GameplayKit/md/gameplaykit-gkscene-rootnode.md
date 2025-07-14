

- GameplayKit
- GKScene
-  rootNode 

Instance Property

# rootNode

The SpriteKit scene managed by this GKScene object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var rootNode: (any GKSceneRootNodeType)? { get set }
```

## Discussion

The GKSceneRootNodeType protocol is an indirect type for game scene classes that the GKScene class can load. SKScene is the only class currently supported for loading with the GKScene class.

