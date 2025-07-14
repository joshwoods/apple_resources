

- ARKit
-  ObjectAnchor 

Structure

# ObjectAnchor

A reference object ARKit is tracking.

visionOS 2.0+

``` source
struct ObjectAnchor
```

## Overview

You use object anchors to learn about the position and orientation of a real-world object.

## Topics

### Inspecting an object anchor

var boundingBox: ObjectAnchor.AxisAlignedBoundingBox

The bounding box of an anchor.

struct AxisAlignedBoundingBox

Values that describe an axis-aligned bounding box.

var description: String

A textual representation of this anchor.

var isTracked: Bool

A Boolean value that indicates whether the framework is currently tracking an object anchor.

var originFromAnchorTransform: simd_float4x4

The transform from the object anchor to the origin coordinate system.

var referenceObject: ReferenceObject

The reference object that an anchor corresponds to.

var inputFile: URL?

The input file the framework uses for loading a reference object.

var usdzFile: URL?

The trained USDZ file, if the reference object includes one.

struct ReferenceObject

An object the framework can track.

### Inspecting and comparing anchors

var id: UUID

The unique identifier of this anchor.

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Conforms To

- Anchor
- CustomStringConvertible
- Equatable
- Identifiable
- Sendable
- TrackableAnchor

## See Also

### Object tracking

class ObjectTrackingProvider

A source of real-time position of reference objects in a person’s environment.

Exploring object tracking with ARKit

Find and track real-world objects in visionOS using reference objects trained with Create ML.

Implementing object tracking in your visionOS app

Create engaging interactions by training models to recognize and track real-world objects in your app.

