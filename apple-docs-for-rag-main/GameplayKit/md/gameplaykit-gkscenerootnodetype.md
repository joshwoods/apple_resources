

- GameplayKit
-  GKSceneRootNodeType 

Protocol

# GKSceneRootNodeType

Identifies scene classes from other frameworks that support embedded GameplayKit information.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
protocol GKSceneRootNodeType : NSObjectProtocol
```

## Overview

You do not define classes that adopt this protocol. GameplayKit adds this protocol declaration to classes (such as SKScene) for which the GKScene class supports archiving and loading embedded GameplayKit information.

For more information, see GameplayKit Programming Guide.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Xcode and SpriteKit Integration

class GKScene

A container for associating GameplayKit objects with a SpriteKit scene.

class GKSKNodeComponent

A component that manages a SpriteKit node.

