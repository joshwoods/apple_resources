

- SpriteKit
- SKAction
-  customAction(withDuration:actionBlock:) 

Type Method

# customAction(withDuration:actionBlock:)

Creates an action that executes a block over a duration.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func customAction(
    withDuration duration: TimeInterval,
    actionBlock block: @escaping (SKNode, CGFloat) -> Void
) -> SKAction
```

## Parameters 

`duration`  

The duration of the action, in seconds.

`block`  

The block to run. The block takes the following parameters:

node  
The node on which the action is running.

elapsedTime  
The amount of time that has passed in the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the block is called repeatedly until the action’s duration expires. The elapsed time is computed and passed to the block whenever the block is called.

This action is not reversible; the reverse action executes the same block.

The following Swift code shows how you can create a custom action to update an attribute of an SKShader attached to a sprite node.

```
let customAction = SKAction.customAction(withDuration: 2.0) {
    node, elapsedTime in

    if let node = node as? SKSpriteNode {
        node.setValue(SKAttributeValue(float: Float(elapsedTime)),
                                       forAttribute: "a_time")
    }
}
```

## See Also

### Creating Custom Actions

init?(named: String)

Creates an action of the given name from an action file.

init?(named: String, duration: TimeInterval)

Creates an action of the given name from an action file with a new duration.

init?(named: String, fromURL: URL)

Creates an action of the given name from an action file.

init?(named: String, fromURL: URL, duration: TimeInterval)

Creates an action of the given name from an action file with a new duration.

class func perform(Selector, onTarget: Any) -> SKAction

Creates an action that calls a method on an object.

class func run(() -> Void) -> SKAction

Creates an action that executes a block.

class func run(() -> Void, queue: dispatch_queue_t) -> SKAction

Creates an action that executes a block on a specific dispatch queue.

