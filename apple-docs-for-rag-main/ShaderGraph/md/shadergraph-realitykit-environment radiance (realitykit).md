

- ShaderGraph
- RealityKit
-  Environment Radiance (RealityKit) 

ShaderGraph Node

# Environment Radiance (RealityKit)

Returns an environment’s diffuse and specular radiance value based on real-world environment, and an IBL map that is either a developer-provided map or a default map.

## Parameter Types

| Input        | Type     |
|--------------|----------|
| `Base Color` | Color3   |
| `Roughness`  | Half     |
| `Specular`   | Half     |
| `Metallic`   | Half     |
| `Normal`     | Vector3f |

| Output              | Type   |
|---------------------|--------|
| `Diffuse Radiance`  | Color3 |
| `Specular Radiance` | Color3 |

## Parameter descriptions

`Base Color`  
The base display color of the surface. The color under pure white light.

`Roughness`  
The level of roughness of the surface. This value ranges between `0` and `1.0`, with `0` representing a perfectly specular surface and `1.0` representing maximum roughness. The default value is `0`.

`Specular`  
The level of specular reflections that occur on the surface.

`Metallic`  
The indicator if a surface is metallic or not. Set this value to `1` for metallic surfaces and `0` for nonmetallic surfaces. The default value is `0.0`.

`Normal`  
The surface normal vector. The default value is `(0,0,0)`.

## Discussion:

The Environment Radiance node has two outputs:

`Diffuse Radiance`  
The diffuse radiance of the surface. Refers to light absorbed by the surface and then re-emitted in all directions.

`Specular Radiance`  
The specular radiance of the surface. Refers to light reflected off of the surface.

## See Also

### Nodes

Unlit Surface (RealityKit)

A surface shader that defines properties for a RealityKit Unlit material.

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

