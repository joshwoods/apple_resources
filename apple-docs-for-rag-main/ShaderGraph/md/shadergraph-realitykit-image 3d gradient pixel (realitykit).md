

- ShaderGraph
- RealityKit
-  Image 3D Gradient Pixel (RealityKit) 

ShaderGraph Node

# Image 3D Gradient Pixel (RealityKit)

A texture with RealityKit properties. Level of detail gradient. Pixel texture coordinates.

## Parameter Types

- Image 3D Gradient Pixel (vector4f)
- Image 3D Gradient Pixel (color3)
- Image 3D Gradient Pixel (color4)

| Input                   | Type      |
|-------------------------|-----------|
| `File`                  | AssetPath |
| `U Wrap Mode`           | String    |
| `V Wrap Mode`           | String    |
| `W Wrap Mode`           | String    |
| `Border Color`          | String    |
| `Filter`                | String    |
| `Max Anisotropy`        | Int32     |
| `Max Lod Clamp`         | Float     |
| `Min Lod Clamp`         | Float     |
| `Default`               | Vector4f  |
| `Texture Coordinates`   | Vector3f  |
| `Dynamic Min Lod Clamp` | Float     |
| `Gradient3D D Pdx`      | Vector3f  |
| `Gradient3D D Pdy`      | Vector3f  |
| `Offset`                | Integer3  |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input                   | Type      |
|-------------------------|-----------|
| `File`                  | AssetPath |
| `U Wrap Mode`           | String    |
| `V Wrap Mode`           | String    |
| `W Wrap Mode`           | String    |
| `Border Color`          | String    |
| `Filter`                | String    |
| `Max Anisotropy`        | Int32     |
| `Max Lod Clamp`         | Float     |
| `Min Lod Clamp`         | Float     |
| `Default`               | Color3    |
| `Texture Coordinates`   | Vector3f  |
| `Dynamic Min Lod Clamp` | Float     |
| `Gradient3D D Pdx`      | Vector3f  |
| `Gradient3D D Pdy`      | Vector3f  |
| `Offset`                | Integer3  |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input                   | Type      |
|-------------------------|-----------|
| `File`                  | AssetPath |
| `U Wrap Mode`           | String    |
| `V Wrap Mode`           | String    |
| `W Wrap Mode`           | String    |
| `Border Color`          | String    |
| `Filter`                | String    |
| `Max Anisotropy`        | Int32     |
| `Max Lod Clamp`         | Float     |
| `Min Lod Clamp`         | Float     |
| `Default`               | Color4    |
| `Texture Coordinates`   | Vector3f  |
| `Dynamic Min Lod Clamp` | Float     |
| `Gradient3D D Pdx`      | Vector3f  |
| `Gradient3D D Pdy`      | Vector3f  |
| `Offset`                | Integer3  |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

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

