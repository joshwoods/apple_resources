

- SpriteKit
- SKWarpGeometryGrid
-  replacingBySourcePositions(positions:) 

Instance Method

# replacingBySourcePositions(positions:)

Returns a copy of this grid, updated with the argument source positions.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
func replacingBySourcePositions(positions source: [SIMD2]) -> SKWarpGeometryGrid
```

## Return Value

A new warp geometry grid.

## See Also

### Accessing or Setting Grid Vertices

func destPosition(at: Int) -> vector_float2

Returns the destination position of a vertex.

func replacingByDestinationPositions(positions: [SIMD2&lt;Float>]) -> SKWarpGeometryGrid

Returns a copy of this grid, updated with the argument destination positions.

func sourcePosition(at: Int) -> vector_float2

Returns the source position of a vertex.

