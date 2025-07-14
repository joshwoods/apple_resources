

- ShaderGraph
- RealityKit
-  Geometry Modifier (RealityKit) 

ShaderGraph Node

# Geometry Modifier (RealityKit)

A function that manipulates the location of a model’s vertices, run once per vertex.

## Parameter Types

| Input                   | Type     |
|-------------------------|----------|
| `Model Position Offset` | Vector3f |
| `Color`                 | Color4   |
| `Normal`                | Vector3f |
| `Bitangent`             | Vector3f |
| `Uv0`                   | Vector2f |
| `Uv1`                   | Vector2f |
| `Uv2`                   | Vector4f |
| `Uv3`                   | Vector4f |
| `Uv4`                   | Vector4f |
| `Uv5`                   | Vector4f |
| `Uv6`                   | Vector4f |
| `Uv7`                   | Vector4f |

| Output | Type  |
|--------|-------|
| `Out`  | Token |

## Parameter descriptions

`Model Position Offset`  
The offset to each vertices model position.

`Color`  
The color of each vertex.

`Normal`  
The normal vector for each vertex.

`Bitangent`  
The bitangent vector for each vertex.

`Uv0`  
A set of texture coordinates for each vertex.

`Uv1`  
A set of texture coordinates for each vertex.

`User Attribute`  
A user-defined attribute to apply to each vertex of the object.

`User Attribute Half4 0`  
A user-defined attribute the node attaches to each vertex of the object.

`User Attribute Half4 1`  
A user-defined attribute the node attaches to each vertex of the object.

`User Attribute Half4 2`  
A user-defined attribute the node attaches to each vertex of the object.

`User Attribute Half4 3`  
A user-defined attribute the node attaches to each vertex of the object.

`User Attribute Half2 0`  
A user-defined attribute the node attaches to each vertex of the object.

`User Attribute Half2 1`  
A user-defined attribute the node attaches to each vertex of the object.

## Discussion

The Geometry Modifier node can be used to cause a material to affect the geometry of any object to which it’s applied, in addition to the objects texture. Connect the output of the Geometry modifier node to the `Custom Geometry Modifier` output of your material. Below is an example of a simple node graph that uses the Geometry Modifier node to alter the *Y* model positions of vertices.

Use the Noise 2D node to procedurally generate an amount to offset the *Y* position of each vertex. You can also use the noise to add shadows to the texture in order to show the change in model position more clearly. Below, the resulting material applies to a plane.

Object before modifier

Object after modifier

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

