

- RealityKit
- MeshResource
-  generateSphere(radius:) 

Type Method

# generateSphere(radius:)

Creates a new sphere mesh with the specified radius.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func generateSphere(radius: Float) -> MeshResource
```

## Parameters 

`radius`  

The radius, in meters, of the sphere.

## Return Value

A sphere mesh.

## Discussion

The sphere is centered at the entity’s origin.

## See Also

### Creating a primitive shape

static func generateCone(height: Float, radius: Float) -> MeshResource

Creates a new cone mesh with the specified dimensions.

static func generateCylinder(height: Float, radius: Float) -> MeshResource

Creates a new cylinder mesh with the specified dimensions.

