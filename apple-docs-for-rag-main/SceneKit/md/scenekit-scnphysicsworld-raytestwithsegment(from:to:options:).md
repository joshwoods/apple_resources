

- SceneKit
- SCNPhysicsWorld
-  rayTestWithSegment(from:to:options:) 

Instance Method

# rayTestWithSegment(from:to:options:)

Searches for physics bodies along a line segment between two points in the physics world.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func rayTestWithSegment(
    from origin: SCNVector3,
    to dest: SCNVector3,
    options: [SCNPhysicsWorld.TestOption : Any]? = nil
) -> [SCNHitTestResult]
```

## Parameters 

`origin`  

An endpoint of the line segment to search, specified in the scene’s world coordinate system.

`dest`  

The other endpoint of the line segment to search, specified in the scene’s world coordinate system.

`options`  

A dictionary of options affecting the test, or `nil` to use default options. For applicable keys and the possible values, see `Physics Test Options Keys`.

## Return Value

An array of SCNHitTestResult objects describing search results.

## Discussion

Use this method to implement concepts such as line of sight in your app. For example, in a game you might implement behavior for an enemy character by searching for physics bodies along a line between the enemy character’s position and the player character’s position, as illustrated below:

```
// Options: Look only for the closest object along line of sight,
// and use the collision bitmask to avoid finding the enemy itself.
NSDictionary *options = @{ SCNPhysicsTestSearchModeKey : SCNPhysicsTestSearchModeClosest,
                     SCNPhysicsTestCollisionBitMaskKey : @(kMyCategoryPlayer) };

NSArray *results = [physicsWorld rayTestWithSegmentFromPoint:enemy.position
                                                     toPoint:player.position
                                                     options:options];
if (results.firstObject.node == player) {
    // Enemy can see player: begin pursuit.
} else {
    // Enemy cannot see player: remain idle.
}
```

## See Also

### Searching for Physics Bodies

func convexSweepTest(with: SCNPhysicsShape, from: SCNMatrix4, to: SCNMatrix4, options: [SCNPhysicsWorld.TestOption : Any]?) -> [SCNPhysicsContact]

Searches for physics bodies in the space formed by moving a convex shape through the physics world.

