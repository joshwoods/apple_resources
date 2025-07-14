

- TabletopKit
- TabletopGame
- TabletopGame.Observer
-  playerChangedSeats(\_:oldSeat:newSeat:snapshot:) 

Instance Method

# playerChangedSeats(\_:oldSeat:newSeat:snapshot:)

Called every time the Seat for any player has changed

visionOS 2.0+

``` source
func playerChangedSeats(
    _ player: Player,
    oldSeat: (any TableSeat)?,
    newSeat: (any TableSeat)?,
    snapshot: TableSnapshot
)
```

**Required** Default implementation provided.

## Default Implementations

### TabletopGame.Observer Implementations

func playerChangedSeats(Player, oldSeat: (any TableSeat)?, newSeat: (any TableSeat)?, snapshot: TableSnapshot)

Called every time the Seat for any player has changed

## See Also

### Handling seat actions

func stateDidResetToBookmark(StateBookmarkIdentifier)

**Required** Default implementation provided.

