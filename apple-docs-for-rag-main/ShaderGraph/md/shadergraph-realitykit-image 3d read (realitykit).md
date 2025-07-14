

- ShaderGraph
- RealityKit
-  Image 3D Read (RealityKit) 

ShaderGraph Node

# Image 3D Read (RealityKit)

Direct texture read.

## Parameter Types

- Image 3D Read (vector4f)
- Image 3D Read (color4)

| Input     | Type      |
|-----------|-----------|
| `File`    | AssetPath |
| `Default` | Vector4f  |
| `X`       | Int32     |
| `Y`       | Int32     |
| `Z`       | Int32     |
| `Lod`     | Int32     |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input     | Type      |
|-----------|-----------|
| `File`    | AssetPath |
| `Default` | Color4    |
| `X`       | Int32     |
| `Y`       | Int32     |
| `Z`       | Int32     |
| `Lod`     | Int32     |

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

