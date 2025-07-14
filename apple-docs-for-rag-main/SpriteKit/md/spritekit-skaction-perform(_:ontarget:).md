

- SpriteKit
- SKAction
-  perform(\_:onTarget:) 

Type Method

# perform(\_:onTarget:)

Creates an action that calls a method on an object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func perform(
    _ selector: Selector,
    onTarget target: Any
) -> SKAction
```

## Parameters 

`selector`  

The selector of the method to call.

`target`  

The target object.

## Return Value

A new action object.

## Discussion

The action object maintains a strong reference to the target object.

When the action executes, the target object’s method is called. This action occurs instantaneously.

This action is not reversible; the reverse of this action calls the selector again.

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

class func customAction(withDuration: TimeInterval, actionBlock: (SKNode, CGFloat) -> Void) -> SKAction

Creates an action that executes a block over a duration.

class func run(() -> Void) -> SKAction

Creates an action that executes a block.

class func run(() -> Void, queue: dispatch_queue_t) -> SKAction

Creates an action that executes a block on a specific dispatch queue.

