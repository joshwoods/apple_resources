

- TabletopKit
- TableVisualState
-  TableVisualState.Contact 

Structure

# TableVisualState.Contact

An object that represents the contact of a collision during a simulation of tossable equipment.

visionOS 2.0+

``` source
struct Contact
```

## Topics

### Getting collision objects

let collider: any Equipment

A dynamic equipment that is in contact with either another equipment or the game’s boundary.

let collidedWithEquipment: EquipmentIdentifier?

The other equipment identifier in contact or `nil` if in contact with the game’s boundary.

### Getting collision metrics

let impulse: Float

Impulse, the force over time of the collision, in newton-seconds.

let normal: Vector3D

The normal of the contacting surfaces at the contact point. The normal direction points from the second shape to the first shape.

let position: Point3D

A position representing the estimated point of contact.

## See Also

### Representing collision states

var contacts: some Sequence&lt;TableVisualState.Contact>

Returns all contacts for the current update of the physics simulation.

func contacts&lt;E>(of: E.Type) -> some Sequence&lt;TableVisualState.Contact> 

Returns all contacts for the current update of the physics simulation for a specified equipment type.

