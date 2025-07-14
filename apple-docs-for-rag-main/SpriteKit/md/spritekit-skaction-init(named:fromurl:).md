

- SpriteKit
- SKAction
-  init(named:fromURL:) 

Initializer

# init(named:fromURL:)

Creates an action of the given name from an action file.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    named name: String,
    fromURL url: URL
)
```

``` source
init?(
    named name: String,
    from url: URL
)
```

## Parameters 

`name`  

The name of the action.

`url`  

The URL of the file containing the action.

## Return Value

A new action object.

## See Also

### Creating Custom Actions

init?(named: String)

Creates an action of the given name from an action file.

init?(named: String, duration: TimeInterval)

Creates an action of the given name from an action file with a new duration.

init?(named: String, fromURL: URL, duration: TimeInterval)

Creates an action of the given name from an action file with a new duration.

class func customAction(withDuration: TimeInterval, actionBlock: (SKNode, CGFloat) -> Void) -> SKAction

Creates an action that executes a block over a duration.

class func perform(Selector, onTarget: Any) -> SKAction

Creates an action that calls a method on an object.

class func run(() -> Void) -> SKAction

Creates an action that executes a block.

class func run(() -> Void, queue: dispatch_queue_t) -> SKAction

Creates an action that executes a block on a specific dispatch queue.

