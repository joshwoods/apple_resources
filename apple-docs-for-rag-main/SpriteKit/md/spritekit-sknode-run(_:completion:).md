

- SpriteKit
- SKNode
-  run(\_:completion:) 

Instance Method

# run(\_:completion:)

Adds an action to the list of actions executed by the node and schedules the argument block to be run upon completion of the action.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
func run(
    _ action: SKAction,
    completion block: @escaping () -> Void
)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func run(
    _ action: SKAction,
    completion block: @escaping () -> Void
)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func run(_ action: SKAction) async
```

**watchOS**

``` source
func run(_ action: SKAction) async
```

## Parameters 

`action`  

The action to perform.

`block`  

A completion block called when the action completes.

## Mentioned in 

Getting Started with Actions

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func run(_ action: SKAction) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Running Actions

Getting Started with Actions

Create, configure, and run actions in SpriteKit.

func run(SKAction)

Adds an action to the list of actions executed by the node.

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

