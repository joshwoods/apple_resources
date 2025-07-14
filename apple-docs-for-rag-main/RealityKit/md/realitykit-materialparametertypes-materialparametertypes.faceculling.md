

- RealityKit
- MaterialParameterTypes
-  MaterialParameterTypes.FaceCulling 

Enumeration

# MaterialParameterTypes.FaceCulling

An object that defines how the system removes polygons before rendering a scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
enum FaceCulling
```

## Overview

To improve performance, RealityKit culls polygons, or faces, that it determines won’t be visible. Discarding faces that aren’t part of the final render eliminates the need to do any calculations for those faces. Use this object to specify what kind of polygons RealityKit culls.

## Topics

### Face culling

case front

The system culls front-facing polygons.

case back

The system culls back-facing polygons.

case none

The system doesn’t cull polygons.

### Comparisons

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

static func == (MaterialParameterTypes.FaceCulling, MaterialParameterTypes.FaceCulling) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

