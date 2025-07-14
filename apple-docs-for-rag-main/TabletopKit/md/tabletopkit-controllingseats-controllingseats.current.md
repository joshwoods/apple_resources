

- TabletopKit
- ControllingSeats
-  ControllingSeats.current 

Case

# ControllingSeats.current

Lets only seats currently in turn interact with the equipment.

visionOS 2.0+

``` source
case current
```

## See Also

### Seats

case any

Lets players in all seats interact with the equipment.

case restricted([TableSeatIdentifier])

Lets players in specific seats interact with the equipment.

case inherited

The value is inherited from the parent. The table implicit value is considered to be `.any`.

