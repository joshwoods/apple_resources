

- TabletopKit
-  TossableRepresentation 

Structure

# TossableRepresentation

An object that represents geometric shapes that the player can throw during gameplay, such as dice.

visionOS 2.0+

``` source
struct TossableRepresentation
```

## Topics

### Creating geometric shapes

static func cube(height: Float, in: UnitLength, restitution: Float?) -> TossableRepresentation

Creates a cube that the player tosses during gameplay.

static func decahedron(height: Float, in: UnitLength, restitution: Float?) -> TossableRepresentation

Creates a decahedron, a symmetrical, ten-faced polyhedron with kite-shaped faces, that the player tosses during gameplay.

static func dodecahedron(height: Float, in: UnitLength, restitution: Float?) -> TossableRepresentation

Creates a regular dodecahedron, a shape with 12 pentagonal faces, that the player tosses during gameplay.

static func icosahedron(height: Float, in: UnitLength, restitution: Float?) -> TossableRepresentation

Creates a regular icosahedron, a shape with 20 triangular faces, that the player tosses during gameplay.

static func octahedron(height: Float, in: UnitLength, restitution: Float?) -> TossableRepresentation

Creates a regular octahedron, a shape with 8 triangular faces, that the player tosses during gameplay.

static func sphere(radius: Float, in: UnitLength, restitution: Float?) -> TossableRepresentation

Creates a sphere with the specified radius that the player tosses during gameplay.

static func tetrahedron(height: Float, in: UnitLength, restitution: Float?) -> TossableRepresentation

Creates a regular tetrahedron, a pyramid with four triangular faces, that the player tosses during gameplay.

## Relationships

### Conforms To

- Sendable

## See Also

### Interactions

class TabletopInteraction

A protocol for objects that manage the entire flow of players interacting with equipment.

struct TableSnapshot

A snapshot of the current state of the table.

struct TableVisualState

A structure that represents the appearance of an object on the table.

struct TableCursor

A visual indicator that represents the destination of player interactions with equipment.

struct TableCursorIdentifier

A unique identifier for cursors.

