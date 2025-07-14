

- SpriteKit
- SKNode
-  removeAction(forKey:) 

Instance Method

# removeAction(forKey:)

Removes an action associated with a specific key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
func removeAction(forKey key: String)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func removeAction(forKey key: String)
```

## Parameters 

`key`  

A string that uniquely identifies an action.

## Mentioned in 

Controlling Actions Precisely by Using Names

## Discussion

If an action is found that matches the key, it is removed from the node.

## See Also

### Running Actions

Getting Started with Actions

Create, configure, and run actions in SpriteKit.

func run(SKAction)

Adds an action to the list of actions executed by the node.

func run(SKAction, completion: () -> Void)

Adds an action to the list of actions executed by the node and schedules the argument block to be run upon completion of the action.

func run(SKAction, withKey: String)

Adds an identifiable action to the list of actions executed by the node.

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

