

- TabletopKit
- TabletopGame
-  TabletopGame.ActionCancellationReason 

Enumeration

# TabletopGame.ActionCancellationReason

The possible reasons for cancelling an action or an interaction.

visionOS 2.0+

``` source
enum ActionCancellationReason
```

## Topics

### Cancellation reasons

case actionInvalidated

The action became invalid due to other cancelled actions

case interactionCancelled

The action was cancelled back because the interaction that generated it got cancelled

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Observing actions

protocol Observer

A protocol for objects that progress gameplay when players take actions.

func addObserver(some TabletopGame.Observer)

func removeObserver(some TabletopGame.Observer)

