

- SpriteKit
- SKNode
-  run(\_:withKey:) 

Instance Method

# run(\_:withKey:)

Adds an identifiable action to the list of actions executed by the node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
func run(
    _ action: SKAction,
    withKey key: String
)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func run(
    _ action: SKAction,
    withKey key: String
)
```

## Parameters 

`action`  

The action to perform.

`key`  

A unique key used to identify the action.

## Mentioned in 

Controlling Actions Precisely by Using Names

## Discussion

This method is identical to run(_:), but the action is stored so that it can be retrieved later. If an action using the same key is already running, it is removed before the new action is added.

## See Also

### Running Actions

Getting Started with Actions

Create, configure, and run actions in SpriteKit.

func run(SKAction)

Adds an action to the list of actions executed by the node.

func run(SKAction, completion: () -> Void)

Adds an action to the list of actions executed by the node and schedules the argument block to be run upon completion of the action.

var speed: CGFloat

A speed modifier applied to all actions executed by a node and its descendants.

var isPaused: Bool

A Boolean value that determines whether actions on the node and its descendants are processed.

func action(forKey: String) -> SKAction?

Returns an action associated with a specific key.

func hasActions() -> Bool

Returns a Boolean value that indicates whether the node is executing actions.

func removeAllActions()

Ends and removes all actions from the node.

func removeAction(forKey: String)

Removes an action associated with a specific key.

