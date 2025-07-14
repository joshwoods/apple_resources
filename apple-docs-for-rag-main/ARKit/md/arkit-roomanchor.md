

- ARKit
-  RoomAnchor 

Structure

# RoomAnchor

The representation of a room ARKit is currently tracking.

visionOS 2.0+

``` source
struct RoomAnchor
```

## Overview

A `RoomAnchor` structure describes an approximate representation of the room’s geometry, and contains arrays with identifiers of mesh and plane anchors that the framework associates with that room.

## Topics

### Getting information about a room anchor

var geometry: MeshAnchor.Geometry

The geometry of the mesh in an anchor’s coordinate system.

var id: UUID

The unique identifier of this anchor.

var isCurrentRoom: Bool

A Boolean value that indicates whether a room is a person’s current location.

var meshAnchorIDs: [UUID]

An array of IDs of the mesh anchors associated with a room.

var originFromAnchorTransform: simd_float4x4

The transform from the room anchor to the origin coordinate system.

var planeAnchorIDs: [UUID]

An array of IDs of the plane anchors associated with a room.

### Inspecting a room anchor

func contains(SIMD3&lt;Float>) -> Bool

Returns a Boolean value that indicates whether a room contains the provided point.

func geometries(of: MeshAnchor.MeshClassification) -> [MeshAnchor.Geometry]

Returns the disjoint mesh geometries of a given classification.

var description: String

A textual representation of this anchor.

## Relationships

### Conforms To

- Anchor
- CustomStringConvertible
- Equatable
- Identifiable
- Sendable

## See Also

### Room tracking

class RoomTrackingProvider

A source of real-time information about the room that a person is currently in.

Building local experiences with room tracking

Use room tracking in visionOS to provide custom interactions with physical spaces.

