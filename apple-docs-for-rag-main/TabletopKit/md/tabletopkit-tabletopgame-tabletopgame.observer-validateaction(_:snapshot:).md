

- TabletopKit
- TabletopGame
- TabletopGame.Observer
-  validateAction(\_:snapshot:) 

Instance Method

# validateAction(\_:snapshot:)

Called locally for local actions Called on the leader for all actions Must be a pure function

visionOS 2.0+

``` source
func validateAction(
    _ action: some TabletopAction,
    snapshot: TableSnapshot
) -> Bool
```

**Required** Default implementation provided.

## Default Implementations

### TabletopGame.Observer Implementations

func validateAction(some TabletopAction, snapshot: TableSnapshot) -> Bool

Called locally for local actions Called on the leader for all actions Must be a pure function

## See Also

### Validating actions

func actionIsPending(some TabletopAction, oldSnapshot: TableSnapshot, newSnapshot: TableSnapshot)

**Required** Default implementation provided.

func actionWasConfirmed(some TabletopAction, oldSnapshot: TableSnapshot, newSnapshot: TableSnapshot)

**Required** Default implementation provided.

func actionWasRolledBack(some TabletopAction, snapshot: TableSnapshot)

**Required** Default implementation provided.

