

- ShaderGraph
- RealityKit
-  Unlit Surface (RealityKit) 

ShaderGraph Node

# Unlit Surface (RealityKit)

A surface shader that defines properties for a RealityKit Unlit material.

## Parameter Types

| Input                         | Type   |
|-------------------------------|--------|
| `Color`                       | Color3 |
| `Opacity`                     | Float  |
| `Opacity Threshold`           | Float  |
| `Apply Post Process Tone Map` | Bool   |
| `Has Premultiplied Alpha`     | Bool   |

| Output | Type  |
|--------|-------|
| `Out`  | Token |

## Parameter descriptions

`Color`  
The base color of the surface.

`Opacity`  
The level of opaqueness of the surface. If the value of this parameter is `1.0`, the surface is fully opaque. If the value is less than `1.0`, the surface appears translucent. If the value is `0`, the surface is completely transparent. The default value is `1.0`.

`Opacity Threshold`  
The threshold for whether the node renders a portion of the surface based on its opacity level. A value of `0.0` means that no additional masking occurs. If the value is greater than `0.0`, the node renders only areas of the surface with an `Opacity` value greater than the value of this parameter. This parameter can be enabled or disabled. The default value is `0.0`.

`Apply Post Process Tone Map`  
A Boolean that tells the node whether to apply the post process tone map.

`Has Premultiplied Alpha`  
A Boolean that tells the node if it has a premultiplied alpha.

## Discussion

The Unlit Surface node produces a custom surface based on its input parameters. Connect the output of the Unlit Surface node connect to the `Custom Surface` output of your material.

## See Also

### Nodes

PBR Surface (RealityKit)

A surface shader that defines properties for a RealityKit Physically Based Rendering material.

Occlusion Surface (RealityKit)

A surface shader that defines properties for a RealityKit Occlusion material that does not receive dynamic lighting.

Shadow Receiving Occlusion Surface (RealityKit)

A surface shader that defines properties for a RealityKit Occlusion material that receives dynamic lighting.

View Direction (RealityKit)

A vector from a position in the scene to the view reference point.

Camera Position (RealityKit)

The position of the camera in the scene.

Geometry Modifier Model To World (RealityKit)

The model-to-world transformation Matrix4x4 (Float).

Geometry Modifier World To Model (RealityKit)

The world-to-model transformation Matrix4x4 (Float).

Geometry Modifier Normal To World (RealityKit)

The normal-to-world transformation Matrix3x3 (Float).

Geometry Modifier Model To View (RealityKit)

The model-to-view transformation Matrix4x4 (Float).

Geometry Modifier View To Projection (RealityKit)

The view-to-projection transformation Matrix4x4 (Float).

Geometry Modifier Projection To View (RealityKit)

The projection-to-view transformation Matrix4x4 (Float).

Geometry Modifier Vertex ID (RealityKit)

The integer index of the vertex.

Surface Model To World (RealityKit)

The model-to-world transformation Matrix4x4 (Float).

Surface Model To View (RealityKit)

The model-to-view transformation Matrix4x4 (Float).

Surface World To View (RealityKit)

The world-to-view transformation Matrix4x4 (Float).

