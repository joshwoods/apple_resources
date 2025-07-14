

- RealityKit
- Entity
-  HasTransform Implementations 

API Collection

# HasTransform Implementations

## Topics

### Instance Properties

var orientation: simd_quatf

The rotation of the entity relative to its parent.

var position: SIMD3&lt;Float>

The position of the entity relative to its parent.

var scale: SIMD3&lt;Float>

The scale of the entity relative to its parent.

var transform: Transform

The transform of an entity relative to its parent.

### Instance Methods

func align(GeometricPin, to: GeometricPin) -> float4x4?

Moves and rotates the entity by a transformation from the origin pin to the target pin.

func convert(direction: SIMD3&lt;Float>, from: Entity?) -> SIMD3&lt;Float>

Converts a direction vector from the local space of a reference entity to the local space of the entity on which you called this method.

func convert(direction: SIMD3&lt;Float>, to: Entity?) -> SIMD3&lt;Float>

Converts a direction vector from the local space of the entity on which you called this method to the local space of a reference entity.

func convert(normal: SIMD3&lt;Float>, from: Entity?) -> SIMD3&lt;Float>

Converts a normal vector from the local space of a reference entity to the local space of the entity on which you called this method.

func convert(normal: SIMD3&lt;Float>, to: Entity?) -> SIMD3&lt;Float>

Converts a normal vector from the local space of the entity on which you called this method to the local space of a reference entity.

func convert(position: SIMD3&lt;Float>, from: Entity?) -> SIMD3&lt;Float>

Converts a position from the local space of a reference entity to the local space of the entity on which you called this method.

func convert(position: SIMD3&lt;Float>, to: Entity?) -> SIMD3&lt;Float>

Converts a position from the local space of the entity on which you called this method to the local space of a reference entity.

func convert(transform: Transform, from: Entity?) -> Transform

Converts the scale, rotation, and position of a transform from the local space of a reference entity to the local space of the entity on which you called this method.

func convert(transform: Transform, to: Entity?) -> Transform

Converts the scale, rotation, and position of a transform from the local space of the entity on which you called this method to the local space of a reference entity.

func look(at: SIMD3&lt;Float>, from: SIMD3&lt;Float>, upVector: SIMD3&lt;Float>, relativeTo: Entity?)

Positions and orients the entity to look at a target from a given position.

func look(at: SIMD3&lt;Float>, from: SIMD3&lt;Float>, upVector: SIMD3&lt;Float>, relativeTo: Entity?, forward: Entity.ForwardDirection)

Positions and orients the entity such that it looks at certain target from a give position.

func move(to: Transform, relativeTo: Entity?)

Moves an entity instantly to a new location given by a transform.

func move(to: float4x4, relativeTo: Entity?)

Moves an entity instantly to a new location given by a 4x4 matrix.

func move(to: float4x4, relativeTo: Entity?, duration: TimeInterval, timingFunction: AnimationTimingFunction) -> AnimationPlaybackController

Moves an entity over a period of time to a new location given by a 4x4 matrix.

func move(to: Transform, relativeTo: Entity?, duration: TimeInterval, timingFunction: AnimationTimingFunction) -> AnimationPlaybackController

Moves an entity over a period of time to a new location given by a transform.

func orientation(relativeTo: Entity?) -> simd_quatf

Gets the orientation of an entity relative to the given entity.

func position(relativeTo: Entity?) -> SIMD3&lt;Float>

Gets the position of an entity relative to the given entity.

func scale(relativeTo: Entity?) -> SIMD3&lt;Float>

Gets the scale of an entity relative to the given entity.

func setOrientation(simd_quatf, relativeTo: Entity?)

Sets the orientation of the entity relative to the given reference entity.

func setPosition(SIMD3&lt;Float>, relativeTo: Entity?)

Sets the position of the entity relative to the given reference entity.

func setScale(SIMD3&lt;Float>, relativeTo: Entity?)

Sets the scale factor of the entity relative to the given reference entity.

func setTransformMatrix(float4x4, relativeTo: Entity?)

Sets the transform of the entity relative to the given reference entity using a 4x4 matrix representation.

func transformMatrix(relativeTo: Entity?) -> float4x4

Gets the 4 x 4 transform matrix of an entity relative to the given entity.

func visualBounds(recursive: Bool, relativeTo: Entity?, excludeInactive: Bool) -> BoundingBox

Computes a bounding box for the entity in the specified space, optionally including child entities.

