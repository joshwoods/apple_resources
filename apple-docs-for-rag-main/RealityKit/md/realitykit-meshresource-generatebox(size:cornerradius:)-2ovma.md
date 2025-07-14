

- RealityKit
- MeshResource
-  generateBox(size:cornerRadius:) 

Type Method

# generateBox(size:cornerRadius:)

Creates a box mesh from a vector of three scalar values that represent width, height, and depth, respectively, and a radius for the corners.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func generateBox(
    size: SIMD3,
    cornerRadius: Float = 0
) -> MeshResource
```

## Parameters 

`size`  

The length of the box’s width, height, and depth, in meters, along the x-, y-, and z-axis, respectively.

`cornerRadius`  

The radius of each corner’s circular arc, in meters. Values for `cornerRadius` can be, at most, equal to `min(size.x, size.y, size.z) / 2.0`. For example, if the box’s dimensions are `3.0` x `4.0` x `5.0`, the corner radius needs to be in the range `[0.0, 1.5]`.

## Discussion

The method centers the box at the entity’s origin and aligns the box’s faces with the coordinate system’s axes.

Note

The method clamps `cornerRadius` so that it doesn’t exceed half the length of the box’s smallest dimension.

## See Also

### Creating a box

static func generateBox(size: Float, cornerRadius: Float) -> MeshResource

Creates a box mesh from a length for the box’s width, height, and depth, and a radius for the corners.

static func generateBox(width: Float, height: Float, depth: Float, cornerRadius: Float, splitFaces: Bool) -> MeshResource

Creates a box mesh from a width, height, depth, a radius for the corners, and a Boolean option that splits faces.

static func generateBox(size: SIMD3&lt;Float>, majorCornerRadius: Float, minorCornerRadius: Float) -> MeshResource

Creates a box mesh from a vector of three scalar values that represent width, height, and depth, respectively, and radii for the corners.

