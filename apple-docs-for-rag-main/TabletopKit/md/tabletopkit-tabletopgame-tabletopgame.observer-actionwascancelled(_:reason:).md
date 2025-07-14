

- TabletopKit
- TabletopGame
- TabletopGame.Observer
-  actionWasCancelled(\_:reason:) 

Instance Method

# actionWasCancelled(\_:reason:)

visionOS 2.0+

``` source
func actionWasCancelled(
    _ action: some TabletopAction,
    reason: TabletopGame.ActionCancellationReason
)
```

**Required** Default implementation provided.

## Default Implementations

### TabletopGame.Observer Implementations

func actionWasCancelled(some TabletopAction, reason: TabletopGame.ActionCancellationReason)

