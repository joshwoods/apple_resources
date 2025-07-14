

- ARKit
-  WorldAnchor 

Structure

# WorldAnchor

A fixed location in a person’s surroundings.

visionOS 1.0+

``` source
struct WorldAnchor
```

## Overview

ARKit persists world anchor UUIDs and transforms across multiple runs of your app. For more information, see Tracking specific points in world space.

## Topics

### Creating a world anchor

init(originFromAnchorTransform: simd_float4x4)

Creates a world anchor from a position and orientation in world space.

### Identifying a world anchor

var id: UUID

The unique identifier of this anchor.

### Inspecting a world anchor

var originFromAnchorTransform: simd_float4x4

The position and orientation of a world anchor.

var isTracked: Bool

A Boolean value that indicates whether ARKit is currently tracking a world anchor.

var description: String

A textual representation of this anchor.

## Relationships

### Conforms To

- Anchor
- Copyable
- CustomStringConvertible
- Equatable
- Identifiable
- Sendable
- TrackableAnchor

## See Also

### World tracking

Tracking specific points in world space

Retrieve the position and orientation of anchors your app stores in ARKit.

class WorldTrackingProvider

A source of live data about the device pose and anchors in a person’s surroundings.

struct DeviceAnchor

The position and orientation of Apple Vision Pro.

