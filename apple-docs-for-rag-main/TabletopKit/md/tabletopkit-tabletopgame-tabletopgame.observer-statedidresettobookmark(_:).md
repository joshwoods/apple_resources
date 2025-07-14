

- TabletopKit
- TabletopGame
- TabletopGame.Observer
-  stateDidResetToBookmark(\_:) 

Instance Method

# stateDidResetToBookmark(\_:)

visionOS 2.0+

``` source
func stateDidResetToBookmark(_ bookmarkID: StateBookmarkIdentifier)
```

**Required** Default implementation provided.

## Default Implementations

### TabletopGame.Observer Implementations

func stateDidResetToBookmark(StateBookmarkIdentifier)

## See Also

### Handling seat actions

func playerChangedSeats(Player, oldSeat: (any TableSeat)?, newSeat: (any TableSeat)?, snapshot: TableSnapshot)

Called every time the Seat for any player has changed

**Required** Default implementation provided.

