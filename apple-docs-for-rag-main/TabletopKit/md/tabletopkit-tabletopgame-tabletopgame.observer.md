

- TabletopKit
- TabletopGame
-  TabletopGame.Observer 

Protocol

# TabletopGame.Observer

A protocol for objects that progress gameplay when players take actions.

visionOS 2.0+

``` source
protocol Observer : AnyObject
```

## Topics

### Handling interaction updates

func interactionWasUpdated(TabletopInteraction.Value, snapshot: TableSnapshot)

Called whenever any player interaction (local or remote) is updated. Remote player interaction updates always include phase `.started` and `.ended` or `.cancelled` but may not include a phase `.update` for every change to the pose or proposedDestination.

**Required** Default implementation provided.

### Validating actions

func validateAction(some TabletopAction, snapshot: TableSnapshot) -> Bool

Called locally for local actions Called on the leader for all actions Must be a pure function

**Required** Default implementation provided.

func actionIsPending(some TabletopAction, oldSnapshot: TableSnapshot, newSnapshot: TableSnapshot)

**Required** Default implementation provided.

func actionWasConfirmed(some TabletopAction, oldSnapshot: TableSnapshot, newSnapshot: TableSnapshot)

**Required** Default implementation provided.

func actionWasRolledBack(some TabletopAction, snapshot: TableSnapshot)

**Required** Default implementation provided.

### Handling seat actions

func playerChangedSeats(Player, oldSeat: (any TableSeat)?, newSeat: (any TableSeat)?, snapshot: TableSnapshot)

Called every time the Seat for any player has changed

**Required** Default implementation provided.

func stateDidResetToBookmark(StateBookmarkIdentifier)

**Required** Default implementation provided.

### Handling cancellations

func actionWasCancelled(some TabletopAction, reason: TabletopGame.ActionCancellationReason)

**Required** Default implementation provided.

## See Also

### Observing actions

func addObserver(some TabletopGame.Observer)

func removeObserver(some TabletopGame.Observer)

enum ActionCancellationReason

The possible reasons for cancelling an action or an interaction.

