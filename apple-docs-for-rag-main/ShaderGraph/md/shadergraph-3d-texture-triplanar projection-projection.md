

- ShaderGraph
- 3D-Texture
-  Triplanar Projection 

ShaderGraph Node

# Triplanar Projection

Samples data from three images and projects each along its respective coordinate axis and blends them by geometric normal.

## Parameter Types

- Triplanar Projection (float)
- Triplanar Projection (vector2f)
- Triplanar Projection (color3f)
- Triplanar Projection (color4f)
- Triplanar Projection (vector4f)
- Triplanar Projection (vector3f)

| Input         | Type      |
|---------------|-----------|
| `File X`      | AssetPath |
| `File Y`      | AssetPath |
| `File Z`      | AssetPath |
| `Default`     | Float     |
| `Position`    | Vector3f  |
| `Normal`      | Vector3f  |
| `Filter Type` | String    |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input         | Type      |
|---------------|-----------|
| `File X`      | AssetPath |
| `File Y`      | AssetPath |
| `File Z`      | AssetPath |
| `Default`     | Vector2f  |
| `Position`    | Vector3f  |
| `Normal`      | Vector3f  |
| `Filter Type` | String    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input         | Type      |
|---------------|-----------|
| `File X`      | AssetPath |
| `File Y`      | AssetPath |
| `File Z`      | AssetPath |
| `Default`     | Color3    |
| `Position`    | Vector3f  |
| `Normal`      | Vector3f  |
| `Filter Type` | String    |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input         | Type      |
|---------------|-----------|
| `File X`      | AssetPath |
| `File Y`      | AssetPath |
| `File Z`      | AssetPath |
| `Default`     | Color4    |
| `Position`    | Vector3f  |
| `Normal`      | Vector3f  |
| `Filter Type` | String    |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input         | Type      |
|---------------|-----------|
| `File X`      | AssetPath |
| `File Y`      | AssetPath |
| `File Z`      | AssetPath |
| `Default`     | Vector4f  |
| `Position`    | Vector3f  |
| `Normal`      | Vector3f  |
| `Filter Type` | String    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input         | Type      |
|---------------|-----------|
| `File X`      | AssetPath |
| `File Y`      | AssetPath |
| `File Z`      | AssetPath |
| `Default`     | Vector3f  |
| `Position`    | Vector3f  |
| `Normal`      | Vector3f  |
| `Filter Type` | String    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

## Parameter Description

`File X`  
The image file to project from the positive *X* direction towards the origin.

`File Y`  
The image file to project from the positive *Y* direction towards the origin.

`File Z`  
The image file to project from the positive *Z* direction towards the origin.

`Default`  
The default value the node uses if any of the ​file​ references fail to resolve.

`Position`  
The 3D coordinates at which the node reads data in order to map the texture onto a surface. The default uses the current 3D object-space coordinates.

`Normal`  
The 3D normal vector the node uses for blending. The default value is the current object-space surface normal.

`Filter Type`  
The type of texture filtering the node uses. The default value is `linear`.

## Discussion

The Triplanar Projection node is used to blend three different images together based on the vector normal of each point on the object. Areas of the object that are parallel with a coordinate axis will cause the node to fully show the respective image. Areas of the object that are in between the coordinate axis will cause the node to render a mix of the images based on how close the normal is to each of the axis. The closer the normal is to being the normal of a coordinate axis the strong the respective image will be in the blend. Below is an example of a simple node graph that uses the Triplanar Projection node to blend the same grass image in the *X* and *Y* directions and a tile texture in the *Z* direction.

Below, the resulting texture applies to a sphere.

