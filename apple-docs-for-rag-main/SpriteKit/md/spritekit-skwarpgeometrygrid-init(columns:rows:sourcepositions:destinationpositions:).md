

- SpriteKit
- SKWarpGeometryGrid
-  init(columns:rows:sourcePositions:destinationPositions:) 

Initializer

# init(columns:rows:sourcePositions:destinationPositions:)

Creates a warp geometry grid of a specific size and warp translation, in point arrays.

iOS 10.0+iPadOS 10.0+Mac CatalystmacOS 10.12+tvOS 10.0+visionOSwatchOS 3.0+

``` source
convenience init(
    columns: Int,
    rows: Int,
    sourcePositions: [SIMD2] = [SIMD2](),
    destinationPositions: [SIMD2] = [SIMD2]()
)
```

## Parameters 

`columns`  

The number of columns in the grid.

`rows`  

The number of rows in the grid.

`sourcePositions`  

Optionally included array of the grid’s source warp positions.

`destinationPositions`  

Optionally included array of the grid’s destination warp positions.

## Return Value

A new warp geometry grid object.

## Discussion

You supply the source and destination position as row-major arrays of normalized vector_float2 coordinates. The number of horizontal coordinates is the column count plus one and the number of vertical coordinates is the row count plus one. Passing `nil` as either of the position arguments results in an identity warp with vertices distributed evenly throughout the geometry. Passing `nil` to both `sourcePositions` and `destPositions` gives a result identical to init(columns:rows:).

## See Also

### Creating a Warp Geometry Grid

convenience init(columns: Int, rows: Int)

Creates a warp geometry grid of a specified size.

init?(coder: NSCoder)

Tells you when to intialize a grid that was loaded from an archive.

