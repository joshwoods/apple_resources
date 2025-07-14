

- RoomPlan
- CapturedRoom
- CapturedRoom.Surface
-  CapturedRoom.Surface.Curve 

Structure

# CapturedRoom.Surface.Curve

An object that represents a single curve of a surface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
struct Curve
```

## Overview

Each CapturedRoom.Surface instance in a captured room’s surface arrays (doors, openings, walls, and windows) that models a curved real-world surface contains an optional property (curve) of this type.

## Topics

### Creating a curve

init(from: any Decoder) throws

Creates a surface curve by deserializing the specified decoder.

### Measuring a curve

var startAngle: Measurement&lt;UnitAngle>

An angle that begins the curve.

var endAngle: Measurement&lt;UnitAngle>

The angle at the end of the curve.

var radius: Float

The radius of the curve.

### Serializing a curve

func encode(to: any Encoder) throws

Serializes a surface curve to the specified encoder.

### Instance Properties

var center: simd_float2

Center of the curve, in local coordinates. Corresponds to xz center coordinates

## Relationships

### Conforms To

- Decodable
- Encodable
- Sendable

## See Also

### Shaping a surface

var completedEdges: Set&lt;CapturedRoom.Surface.Edge>

An array of edges that outline the surface.

enum Edge

An object that represents a single edge of a surface.

var curve: CapturedRoom.Surface.Curve?

An object that represents the curve of a surface.

var polygonCorners: [simd_float3]

A 2D polygon that represents nonuniform wall heights and floor shapes.

