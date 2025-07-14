

- SpriteKit
- SKAction
-  run(\_:queue:) 

Type Method

# run(\_:queue:)

Creates an action that executes a block on a specific dispatch queue.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func run(
    _ block: @escaping () -> Void,
    queue: dispatch_queue_t
) -> SKAction
```

## Parameters 

`block`  

The block to run.

`queue`  

The queue to perform the action on.

## Return Value

A new action object.

## Discussion

When the action executes, the block is called. This action takes place instantaneously.

This action is not reversible; the reverse action executes the same block.

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

class func perform(Selector, onTarget: Any) -> SKAction

Creates an action that calls a method on an object.

class func run(() -> Void) -> SKAction

Creates an action that executes a block.

