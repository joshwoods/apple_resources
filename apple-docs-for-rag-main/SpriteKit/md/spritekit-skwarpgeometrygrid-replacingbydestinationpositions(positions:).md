

- SpriteKit
- SKWarpGeometryGrid
-  replacingByDestinationPositions(positions:) 

Instance Method

# replacingByDestinationPositions(positions:)

Returns a copy of this grid, updated with the argument destination positions.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
func replacingByDestinationPositions(positions destination: [SIMD2]) -> SKWarpGeometryGrid
```

## Return Value

A new warp geometry grid.

## See Also

### Accessing or Setting Grid Vertices

func destPosition(at: Int) -> vector_float2

Returns the destination position of a vertex.

func replacingBySourcePositions(positions: [SIMD2&lt;Float>]) -> SKWarpGeometryGrid

Returns a copy of this grid, updated with the argument source positions.

func sourcePosition(at: Int) -> vector_float2

Returns the source position of a vertex.

