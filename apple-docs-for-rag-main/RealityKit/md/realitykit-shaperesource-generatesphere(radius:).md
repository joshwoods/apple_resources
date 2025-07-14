

- RealityKit
- ShapeResource
-  generateSphere(radius:) 

Type Method

# generateSphere(radius:)

Creates a sphere shape with the specified radius.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func generateSphere(radius: Float) -> ShapeResource
```

## Parameters 

`radius`  

The radius of the sphere in meters.

## Return Value

The new sphere centered at the local origin.

## Discussion

Note

Collision shape extents that fall below 2mm are forced to be 2mm in size - this includes, entities with negative scale values.

