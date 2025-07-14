

- SpriteKit
-  SKWarpGeometryGrid 

Class

# SKWarpGeometryGrid

A definition for a grid-based deformation of nodes that conform to SKWarpable.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class SKWarpGeometryGrid
```

## Mentioned in 

Animate the Warping of a Sprite

Warping SpriteKit Content By Using an Effect Node

## Overview

An `SKWarpGeometryGrid` exposes a 2D array of source positions, and set of destination positions with matching size, that allow you to define which sections of a node should be translated from the source positions to the destination positions. Conceptually, this forms two grids—a source grid and a destination grid—where the visual warping is accomplished by stretching or shrinking each section of the node as the source positions of the grid interpolate to their corresponding destination positions.

## Topics

### Creating a Warp Geometry Grid

convenience init(columns: Int, rows: Int)

Creates a warp geometry grid of a specified size.

convenience init(columns: Int, rows: Int, sourcePositions: [SIMD2&lt;Float>], destinationPositions: [SIMD2&lt;Float>])

Creates a warp geometry grid of a specific size and warp translation, in point arrays.

init?(coder: NSCoder)

Tells you when to intialize a grid that was loaded from an archive.

### Animating Warping

Animate the Warping of a Sprite

Interpolate warping from source to destination warp geometry grids.

### Accessing or Setting Warp Geometry Grid Size

var numberOfColumns: Int

The object’s number of columns.

var numberOfRows: Int

The object’s number of rows.

var vertexCount: Int

The object’s total number of vertices.

### Accessing or Setting Grid Vertices

Get or set `float2` values that correspond to individual vertices of the grid.

func destPosition(at: Int) -> vector_float2

Returns the destination position of a vertex.

func replacingByDestinationPositions(positions: [SIMD2&lt;Float>]) -> SKWarpGeometryGrid

Returns a copy of this grid, updated with the argument destination positions.

func replacingBySourcePositions(positions: [SIMD2&lt;Float>]) -> SKWarpGeometryGrid

Returns a copy of this grid, updated with the argument source positions.

func sourcePosition(at: Int) -> vector_float2

Returns the source position of a vertex.

## Relationships

### Inherits From

- SKWarpGeometry

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Warping

class SKWarpGeometry

A definition for a deformation of nodes that conform to SKWarpable.

protocol SKWarpable

A protocol for objects that can be warped and animated by an SKWarpGeometry.

