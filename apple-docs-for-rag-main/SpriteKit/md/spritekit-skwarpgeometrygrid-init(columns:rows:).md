

- SpriteKit
- SKWarpGeometryGrid
-  init(columns:rows:) 

Initializer

# init(columns:rows:)

Creates a warp geometry grid of a specified size.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
convenience init(
    columns cols: Int,
    rows: Int
)
```

## Parameters 

`cols`  

The number of columns in the grid.

`rows`  

The number of rows in the grid.

## Return Value

A new warp geometry grid object.

## Mentioned in 

Animate the Warping of a Sprite

## Discussion

Creating a warp geometry grid without explicit source and destination positions automatically generates the required position arrays. For example, a 2 column by 2 row grid would create two arrays containing nine positions each, beginning at `[0,0]` - for the bottom left position - and ending at `[1,1]` - for the top left position.

| index: 6, position: \[0.0, 1.0\] | index: 7, position: \[0.5, 1.0\] | index: 8, position: \[1.0, 1.0\] |
|----|----|----|
| index: 3, position: \[0.0, 0.5\] | index: 4, position: \[0.5, 0.5\] | index: 5, position: \[1.0, 0.5\] |
| index: 0, position: \[0.0, 0.0\] | index: 1, position: \[0.5, 0.0\] | index: 2, position: \[1.0, 0.0\] |

## See Also

### Creating a Warp Geometry Grid

convenience init(columns: Int, rows: Int, sourcePositions: [SIMD2&lt;Float>], destinationPositions: [SIMD2&lt;Float>])

Creates a warp geometry grid of a specific size and warp translation, in point arrays.

init?(coder: NSCoder)

Tells you when to intialize a grid that was loaded from an archive.

