

- SpriteKit
- SKNode
-  run(\_:) 

Instance Method

# run(\_:)

Adds an action to the list of actions executed by the node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func run(_ action: SKAction)
```

**watchOS**

``` source
func run(_ action: SKAction)
```

## Parameters 

`action`  

The action to perform.

## Mentioned in 

Getting Started with Actions

## Discussion

The new action is processed the next time the scene’s animation loop is processed.

## See Also

### Running Actions

Getting Started with Actions

Create, configure, and run actions in SpriteKit.

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

func removeAction(forKey: String)

Removes an action associated with a specific key.

