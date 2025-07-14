

- TabletopKit
- ControllingSeats
-  ControllingSeats.restricted(\_:) 

Case

# ControllingSeats.restricted(\_:)

Lets players in specific seats interact with the equipment.

visionOS 2.0+

``` source
case restricted([TableSeatIdentifier])
```

## See Also

### Seats

case any

Lets players in all seats interact with the equipment.

case inherited

The value is inherited from the parent. The table implicit value is considered to be `.any`.

case current

Lets only seats currently in turn interact with the equipment.

