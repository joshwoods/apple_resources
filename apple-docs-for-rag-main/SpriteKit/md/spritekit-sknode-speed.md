

- SpriteKit
- SKNode
-  speed 

Instance Property

# speed

A speed modifier applied to all actions executed by a node and its descendants.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var speed: CGFloat { get set }
```

**watchOS**

``` source
var speed: CGFloat { get set }
```

## Mentioned in 

About Node Property Propagation

## Discussion

The default value is `1.0`, which means that all actions run at their normal speed. If you set a different speed, time appears to run faster or slower for all actions executed on the node and its descendants. For example, if you set a speed value of `2.0`, actions run twice as fast.

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

