

- SpriteKit
- SKPhysicsBody
-  Creating an Edge Loop Around a Scene 

Article

# Creating an Edge Loop Around a Scene

Border your scene with an obstacle that physics bodies cannot penetrate.

## Overview

When you want to confine your in-app objects to a specific region, use an edge-based physics body to define the area. In an app that models a pool table, for example, the balls are the in-app objects, and the table edges collectively create an *edge loop*. The following code demonstrates creating an edge loop to implement an impenetrable boundary that extends from edge to edge in the scene.

- Swift
- Obj-C

```
func createSceneContents() {
    self.backgroundColor = .black
    self.scaleMode = .aspectFit
    self.physicsBody = SKPhysicsBody(edgeLoopFrom: self.frame)
}
```

```
- (void) createSceneContents
{
    self.backgroundColor = [SKColor blackColor];
    self.scaleMode = SKSceneScaleModeAspectFit;
    self.physicsBody = [SKPhysicsBody bodyWithEdgeLoopFromRect:self.frame];
}
```

## See Also

### Creating an Edge-Based Physics Body

init(edgeLoopFrom: CGRect)

Creates an edge loop from a rectangle.

init(edgeFrom: CGPoint, to: CGPoint)

Creates an edge between two points.

init(edgeLoopFrom: CGPath)

Creates an edge loop from a path.

init(edgeChainFrom: CGPath)

Creates an edge chain from a path.

