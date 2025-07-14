

- SpriteKit
- SKAction
-  run(\_:) 

Type Method

# run(\_:)

Creates an action that executes a block.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func run(_ block: @escaping () -> Void) -> SKAction
```

## Parameters 

`block`  

The block to run.

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

class func run(() -> Void, queue: dispatch_queue_t) -> SKAction

Creates an action that executes a block on a specific dispatch queue.

