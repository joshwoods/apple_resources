

- RealityKit
- MeshResource
-  generatePlane(width:height:cornerRadius:) 

Type Method

# generatePlane(width:height:cornerRadius:)

Creates a new rectangle mesh with the specified dimensions in the entity’s xy-plane.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func generatePlane(
    width: Float,
    height: Float,
    cornerRadius: Float = 0
) -> MeshResource
```

## Parameters 

`width`  

The width, in meters, of the rectangle along the x-axis.

`height`  

The height, in meters, of the rectangle along the y-axis.

`cornerRadius`  

A corner radius in the form of a circular arc, with curvature that transitions abruptly from `0` to `1/r` at the boundary between the edge and the corner.

## Return Value

The rectangle mesh.

## Discussion

The rectangle is centered at the entity’s origin and aligned with its x and y axes. The surface normal points along the z-axis. The depth along the z-axis is 0.

Note

The xy-plane is a plane that aligns with the x and y axes.

## See Also

### Creating a plane

static func generatePlane(width: Float, depth: Float, cornerRadius: Float) -> MeshResource

Creates a new rectangle mesh with the specified dimensions in the entity’s xz-plane.

