

- RoomPlan
- CapturedRoom
- CapturedRoom.Surface
-  CapturedRoom.Surface.Edge 

Enumeration

# CapturedRoom.Surface.Edge

An object that represents a single edge of a surface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
enum Edge
```

## Overview

Each CapturedRoom.Surface instance in a captured room’s surface arrays (doors, openings, walls, and windows) has a set (completedEdges) that contains one of each case in this enumeration.

## Topics

### Creating an edge

init(from: any Decoder) throws

Creates a surface edge by deserializing the specified decoder.

### Accessing edge types

case top

An edge that identifies the top of a surface.

case bottom

An edge that identifies the bottom of a surface.

case left

An edge that identifies the left side of a surface.

case right

An edge that identifies the right side of a surface.

static var allCases: [CapturedRoom.Surface.Edge]

A collection of all values of this type.

typealias AllCases

A type that can represent a collection of all values of this type.

### Comparing edges

static func == (CapturedRoom.Surface.Edge, CapturedRoom.Surface.Edge) -> Bool

Determines whether two surface edges are equal.

static func != (Self, Self) -> Bool

Determines whether two surface edges aren’t equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

var hashValue: Int

The hash value.

### Serializing an edge

func encode(to: any Encoder) throws

Serializes a surface edge to the specified encoder.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CaseIterable
- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Shaping a surface

var completedEdges: Set&lt;CapturedRoom.Surface.Edge>

An array of edges that outline the surface.

var curve: CapturedRoom.Surface.Curve?

An object that represents the curve of a surface.

struct Curve

An object that represents a single curve of a surface.

var polygonCorners: [simd_float3]

A 2D polygon that represents nonuniform wall heights and floor shapes.

