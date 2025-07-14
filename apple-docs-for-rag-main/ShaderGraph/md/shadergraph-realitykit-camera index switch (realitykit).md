

- ShaderGraph
- RealityKit
-  Camera Index Switch (RealityKit) 

ShaderGraph Node

# Camera Index Switch (RealityKit)

Render different results for each eye in a stereoscopic render.

## Parameter Types

- Camera Index Switch (integer)
- Camera Index Switch (vector4f)
- Camera Index Switch (color4f)
- Camera Index Switch (color3f)
- Camera Index Switch (vector3f)
- Camera Index Switch (vector2f)
- Camera Index Switch (float)

| Input   | Type  |
|---------|-------|
| `Mono`  | Int32 |
| `Left`  | Int32 |
| `Right` | Int32 |

| Output | Type  |
|--------|-------|
| `Out`  | Int32 |

| Input   | Type     |
|---------|----------|
| `Mono`  | Vector4f |
| `Left`  | Vector4f |
| `Right` | Vector4f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input   | Type   |
|---------|--------|
| `Mono`  | Color4 |
| `Left`  | Color4 |
| `Right` | Color4 |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input   | Type   |
|---------|--------|
| `Mono`  | Color3 |
| `Left`  | Color3 |
| `Right` | Color3 |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input   | Type     |
|---------|----------|
| `Mono`  | Vector3f |
| `Left`  | Vector3f |
| `Right` | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input   | Type     |
|---------|----------|
| `Mono`  | Vector2f |
| `Left`  | Vector2f |
| `Right` | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input   | Type  |
|---------|-------|
| `Mono`  | Float |
| `Left`  | Float |
| `Right` | Float |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

## Parameter descriptions

`Mono`  
The value to return if using a single renderer.

`Left`  
The value to return if seeing the texture through the left eye of a stereoscopic render.

`Right`  
The value to return if seeing the texture through the right eye of a stereoscopic render.

## Discussion

Use the Camera Index Switch node to render stereoscopic images. On most devices, this node simply returns its `Mono` input paramter. On Vision Pro, this node outputs either `Left` or `Right`, depending on which eye the texture renders through.

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

