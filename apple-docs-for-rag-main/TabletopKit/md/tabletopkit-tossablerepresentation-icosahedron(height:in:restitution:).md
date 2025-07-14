

- TabletopKit
- TossableRepresentation
-  icosahedron(height:in:restitution:) 

Type Method

# icosahedron(height:in:restitution:)

Creates a regular icosahedron, a shape with 20 triangular faces, that the player tosses during gameplay.

visionOS 2.0+

``` source
static func icosahedron(
    height: Float,
    in unit: UnitLength = .meters,
    restitution: Float? = nil
) -> TossableRepresentation
```

## Parameters 

`height`  

The height of the icosahedron from face to opposite face.

`unit`  

The unit of measurement for the height.

`restitution`  

The coefficient of restitution, in the range \[0, 1\].

## Discussion

The vertices for the simulated icosahedron with given face to opposite face height (h) are derived from the points on the circumscribed sphere with radius (r) with the following coordinates: phi = (sqrt(5) + 1) / 2, r = h/2 ⋅ sqrt(phi^2 + 1)⋅sqrt(3)/phi^2: ±Y face: ±{ 0, +1, -2/phi^2 } ⋅ h/2, ±{+1/phi^2, +1, +sqrt(3)/phi^2 } ⋅ h/2, ±{+1/phi^2, +1, -sqrt(3)/phi^2 } ⋅ h/2 Equator: ±{ 0, +1/phi^3, 2/phi } ⋅ h/2, ±{ -1/phi, +1/phi^3, +sqrt(3)/phi } ⋅ h/2, ±{ -1/phi, +1/phi^3, -sqrt(3)/phi } ⋅ h/2

Higher restitution values indicate materials that conserve kinetic energy during collisions, causing objects to bounce off each other elastically. Lower values suggest materials that absorb kinetic energy, resulting in less bounce and more energy loss upon impact.

## See Also

### Creating geometric shapes

static func cube(height: Float, in: UnitLength, restitution: Float?) -> TossableRepresentation

Creates a cube that the player tosses during gameplay.

static func decahedron(height: Float, in: UnitLength, restitution: Float?) -> TossableRepresentation

Creates a decahedron, a symmetrical, ten-faced polyhedron with kite-shaped faces, that the player tosses during gameplay.

static func dodecahedron(height: Float, in: UnitLength, restitution: Float?) -> TossableRepresentation

Creates a regular dodecahedron, a shape with 12 pentagonal faces, that the player tosses during gameplay.

static func octahedron(height: Float, in: UnitLength, restitution: Float?) -> TossableRepresentation

Creates a regular octahedron, a shape with 8 triangular faces, that the player tosses during gameplay.

static func sphere(radius: Float, in: UnitLength, restitution: Float?) -> TossableRepresentation

Creates a sphere with the specified radius that the player tosses during gameplay.

static func tetrahedron(height: Float, in: UnitLength, restitution: Float?) -> TossableRepresentation

Creates a regular tetrahedron, a pyramid with four triangular faces, that the player tosses during gameplay.

