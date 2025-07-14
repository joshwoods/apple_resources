

- SpriteKit
- SKNode
-  removeAllActions() 

Instance Method

# removeAllActions()

Ends and removes all actions from the node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func removeAllActions()
```

**watchOS**

``` source
func removeAllActions()
```

## Mentioned in 

Configuring Action Timing

## Discussion

When an action is removed from the node, any remaining animation the action would perform is skipped; however, previous changes are not reverted. It is possible that an action may make a final change to the scene when removed; if so, it is documented for the specific action in SKAction.

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

func removeAction(forKey: String)

Removes an action associated with a specific key.

