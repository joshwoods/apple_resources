

- SpriteKit
- SKWarpGeometryGrid
-  sourcePosition(at:) 

Instance Method

# sourcePosition(at:)

Returns the source position of a vertex.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func sourcePosition(at index: Int) -> vector_float2
```

## Parameters 

`index`  

The index of the position vertex to query.

## Return Value

The normalized position of the specified vertex in `sourcePositions`.

## Discussion

The specified index must be between 0 and the warp geometry grid’s vertexCount `- 1`.

## See Also

### Accessing or Setting Grid Vertices

func destPosition(at: Int) -> vector_float2

Returns the destination position of a vertex.

func replacingByDestinationPositions(positions: [SIMD2&lt;Float>]) -> SKWarpGeometryGrid

Returns a copy of this grid, updated with the argument destination positions.

func replacingBySourcePositions(positions: [SIMD2&lt;Float>]) -> SKWarpGeometryGrid

Returns a copy of this grid, updated with the argument source positions.

