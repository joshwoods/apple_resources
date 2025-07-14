

- TabletopKit
- TableVisualState
-  contacts(of:) 

Instance Method

# contacts(of:)

Returns all contacts for the current update of the physics simulation for a specified equipment type.

visionOS 2.0+

``` source
func contacts(of type: E.Type) -> some Sequence where E : Equipment
```

## See Also

### Representing collision states

var contacts: some Sequence&lt;TableVisualState.Contact>

Returns all contacts for the current update of the physics simulation.

struct Contact

An object that represents the contact of a collision during a simulation of tossable equipment.

