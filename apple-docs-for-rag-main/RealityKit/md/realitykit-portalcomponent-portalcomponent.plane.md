

- RealityKit
- PortalComponent
-  PortalComponent.Plane 

Structure

# PortalComponent.Plane

A representation of a portal as an infinite plane.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Plane
```

## Overview

Enable the corresponding clipping and crossing features by passing this value in PortalComponent.ClippingMode.plane(_:) or PortalComponent.CrossingMode.plane(_:).

RealityKit defines the position and normal properties in entity local space.

The following default values are available:

- positiveX

- negativeX

- positiveY

- negativeY

- positiveZ

- negativeZ

See PortalComponent for example usage.

## Topics

### Operators

static func == (PortalComponent.Plane, PortalComponent.Plane) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(position: SIMD3&lt;Float>, normal: SIMD3&lt;Float>)

Creates a portal plane with position and normal.

### Instance Properties

var normal: SIMD3&lt;Float>

The normal of the portal plane, in entity local space.

var position: SIMD3&lt;Float>

The position of the portal plane, in entity local space.

### Type Properties

static let negativeX: PortalComponent.Plane

A portal plane sitting at the origin facing the negative x direction.

static let negativeY: PortalComponent.Plane

A portal plane sitting at the origin facing the negative y direction.

static let negativeZ: PortalComponent.Plane

A portal plane sitting at the origin facing the negative z direction.

static let positiveX: PortalComponent.Plane

A portal plane sitting at the origin facing the positive x direction.

static let positiveY: PortalComponent.Plane

A portal plane sitting at the origin facing the positive y direction.

static let positiveZ: PortalComponent.Plane

A portal plane sitting at the origin facing the positive z direction.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

