

- RealityKit
- Views and attachments
- RealityViewCameraContent
-  RealityCoordinateSpaceProjecting Implementations 

API Collection

# RealityCoordinateSpaceProjecting Implementations

## Topics

### Instance Methods

func entities(at: CGPoint, in: some CoordinateSpaceProtocol) -> [Entity]

Finds all the hit entities when projecting a ray from a starting point.

func entity(at: CGPoint, in: some CoordinateSpaceProtocol) -> Entity?

Finds the first entity hit when projecting a ray from a starting point.

func hitTest(point: CGPoint, in: some CoordinateSpaceProtocol, query: CollisionCastQueryType, mask: CollisionGroup) -> [CollisionCastHit]

Searches the scene for entities at the specified point in the view.

func project(point: SIMD3&lt;Float>, to: some CoordinateSpaceProtocol) -> CGPoint?

Projects a point from the 3D world coordinate system of the scene to the 2D pixel coordinate system of the reality view.

func ray(through: CGPoint, in: some CoordinateSpaceProtocol, to: some RealityCoordinateSpace) -> (origin: SIMD3&lt;Float>, direction: SIMD3&lt;Float>)?

Determines the position and direction of a ray through the given point in the 2D space of the view.

func unproject(CGPoint, from: some CoordinateSpaceProtocol, to: some RealityCoordinateSpace, ontoPlane: float4x4) -> SIMD3&lt;Float>?

Unprojects a point from the view onto a plane in 3D world coordinates.

