

- TabletopKit
- TabletopGame
-  claimAnySeat() 

Instance Method

# claimAnySeat()

Claims any free seat. If there are no free seats, it has no effect

visionOS 2.0+

``` source
func claimAnySeat()
```

## See Also

### Managing seats

func claimSeat(some TableSeat)

Claims the given seat. If provided Seat is not part of the table, it has no effect

func claimSeat(matching: TableSeatIdentifier)

Claims the given seat. If provided ID does not exist, it has no effect

func releaseSeat()

Releases the seat for this player. If the player is not seated it has no effect

