

- TabletopKit
- TabletopGame
- TabletopGame.Observer
-  actionWasConfirmed(\_:oldSnapshot:newSnapshot:) 

Instance Method

# actionWasConfirmed(\_:oldSnapshot:newSnapshot:)

visionOS 2.0+

``` source
func actionWasConfirmed(
    _ action: some TabletopAction,
    oldSnapshot: TableSnapshot,
    newSnapshot: TableSnapshot
)
```

**Required** Default implementation provided.

## Default Implementations

### TabletopGame.Observer Implementations

func actionWasConfirmed(some TabletopAction, oldSnapshot: TableSnapshot, newSnapshot: TableSnapshot)

## See Also

### Validating actions

func validateAction(some TabletopAction, snapshot: TableSnapshot) -> Bool

Called locally for local actions Called on the leader for all actions Must be a pure function

**Required** Default implementation provided.

func actionIsPending(some TabletopAction, oldSnapshot: TableSnapshot, newSnapshot: TableSnapshot)

**Required** Default implementation provided.

func actionWasRolledBack(some TabletopAction, snapshot: TableSnapshot)

**Required** Default implementation provided.

