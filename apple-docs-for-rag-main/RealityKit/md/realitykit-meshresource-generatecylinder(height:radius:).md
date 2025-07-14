

- RealityKit
- MeshResource
-  generateCylinder(height:radius:) 

Type Method

# generateCylinder(height:radius:)

Creates a new cylinder mesh with the specified dimensions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
static func generateCylinder(
    height: Float,
    radius: Float
) -> MeshResource
```

## Parameters 

`height`  

The height of the cylinder in meters \[m\].

`radius`  

The radius of the cylinder in meters \[m\].

## Discussion

The cylinder is centered at the local origin.

## See Also

### Creating a primitive shape

static func generateSphere(radius: Float) -> MeshResource

Creates a new sphere mesh with the specified radius.

static func generateCone(height: Float, radius: Float) -> MeshResource

Creates a new cone mesh with the specified dimensions.

