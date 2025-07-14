

- SpriteKit
- SKNode
-  hasActions() 

Instance Method

# hasActions()

Returns a Boolean value that indicates whether the node is executing actions.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func hasActions() -> Bool
```

**watchOS**

``` source
func hasActions() -> Bool
```

## Return Value

true if the node has any executing actions; otherwise false.

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

func removeAllActions()

Ends and removes all actions from the node.

func removeAction(forKey: String)

Removes an action associated with a specific key.

