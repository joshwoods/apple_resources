

- SpriteKit
- SKWarpGeometryGrid
-  init(coder:) 

Initializer

# init(coder:)

Tells you when to intialize a grid that was loaded from an archive.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init?(coder aDecoder: NSCoder)
```

## See Also

### Creating a Warp Geometry Grid

convenience init(columns: Int, rows: Int)

Creates a warp geometry grid of a specified size.

convenience init(columns: Int, rows: Int, sourcePositions: [SIMD2&lt;Float>], destinationPositions: [SIMD2&lt;Float>])

Creates a warp geometry grid of a specific size and warp translation, in point arrays.

