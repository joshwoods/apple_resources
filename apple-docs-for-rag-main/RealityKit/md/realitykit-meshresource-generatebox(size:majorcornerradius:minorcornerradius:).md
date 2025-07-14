

- RealityKit
- MeshResource
-  generateBox(size:majorCornerRadius:minorCornerRadius:) 

Type Method

# generateBox(size:majorCornerRadius:minorCornerRadius:)

Creates a box mesh from a vector of three scalar values that represent width, height, and depth, respectively, and radii for the corners.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
static func generateBox(
    size: SIMD3,
    majorCornerRadius: Float = 0.2,
    minorCornerRadius: Float = 0.05
) -> MeshResource
```

## Parameters 

`size`  

The length of the box’s width, height, and depth, in meters, along the x-, y-, and z-axis, respectively.

`majorCornerRadius`  

The radius of each corner’s circular arc, in meters, orthogonal to the z-axis.

`minorCornerRadius`  

The radius of each corner’s circular arc, in meters, orthogonal to the x-axis.

## Discussion

The method centers the box at the entity’s origin and aligns the box’s faces with the coordinate system’s axes.

## See Also

### Creating a box

static func generateBox(size: Float, cornerRadius: Float) -> MeshResource

Creates a box mesh from a length for the box’s width, height, and depth, and a radius for the corners.

static func generateBox(size: SIMD3&lt;Float>, cornerRadius: Float) -> MeshResource

Creates a box mesh from a vector of three scalar values that represent width, height, and depth, respectively, and a radius for the corners.

static func generateBox(width: Float, height: Float, depth: Float, cornerRadius: Float, splitFaces: Bool) -> MeshResource

Creates a box mesh from a width, height, depth, a radius for the corners, and a Boolean option that splits faces.

