

- TabletopKit
- TabletopGame
- TabletopGame.Observer
-  actionWasRolledBack(\_:snapshot:) 

Instance Method

# actionWasRolledBack(\_:snapshot:)

visionOS 2.0+

``` source
func actionWasRolledBack(
    _ action: some TabletopAction,
    snapshot: TableSnapshot
)
```

**Required** Default implementation provided.

## Default Implementations

### TabletopGame.Observer Implementations

func actionWasRolledBack(some TabletopAction, snapshot: TableSnapshot)

## See Also

### Validating actions

func validateAction(some TabletopAction, snapshot: TableSnapshot) -> Bool

Called locally for local actions Called on the leader for all actions Must be a pure function

**Required** Default implementation provided.

func actionIsPending(some TabletopAction, oldSnapshot: TableSnapshot, newSnapshot: TableSnapshot)

**Required** Default implementation provided.

func actionWasConfirmed(some TabletopAction, oldSnapshot: TableSnapshot, newSnapshot: TableSnapshot)

**Required** Default implementation provided.

