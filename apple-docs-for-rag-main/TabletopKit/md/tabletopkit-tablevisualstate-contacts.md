

- TabletopKit
- TableVisualState
-  contacts 

Instance Property

# contacts

Returns all contacts for the current update of the physics simulation.

visionOS 2.0+

``` source
var contacts: some Sequence { get }
```

## See Also

### Representing collision states

func contacts&lt;E>(of: E.Type) -> some Sequence&lt;TableVisualState.Contact> 

Returns all contacts for the current update of the physics simulation for a specified equipment type.

struct Contact

An object that represents the contact of a collision during a simulation of tossable equipment.

