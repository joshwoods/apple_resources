

- ARKit
-  EnvironmentProbeAnchor 

Structure

# EnvironmentProbeAnchor

An environment probe in the world.

visionOS 2.0+

``` source
struct EnvironmentProbeAnchor
```

## Overview

Use environment probes to light virtual geometry by producing environment textures from the probe’s location in the world.

Note

The framework always positions the anchor at the location of the Vision Pro device.

## Topics

### Getting anchor information

var environmentTexture: (any MTLTexture)?

The environment texture of an anchor.

var cameraScaleReference: Float

The camera scale reference of this anchor.

var originFromAnchorTransform: simd_float4x4

The transform from the environment probe anchor to the origin coordinate system.

### Comparing environment probe anchors

var id: UUID

The unique identifier of this anchor.

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

### Lighting estimation

class EnvironmentLightEstimationProvider

A source of live data about lighting information in the environment.

