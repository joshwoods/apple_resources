

- ARKit
- RoomAnchor
-  id 

Instance Property

# id

The unique identifier of this anchor.

visionOS 2.0+

``` source
var id: UUID { get }
```

## See Also

### Getting information about a room anchor

var geometry: MeshAnchor.Geometry

The geometry of the mesh in an anchor’s coordinate system.

var isCurrentRoom: Bool

A Boolean value that indicates whether a room is a person’s current location.

var meshAnchorIDs: [UUID]

An array of IDs of the mesh anchors associated with a room.

var originFromAnchorTransform: simd_float4x4

The transform from the room anchor to the origin coordinate system.

var planeAnchorIDs: [UUID]

An array of IDs of the plane anchors associated with a room.

