

- ShaderGraph
- Organization
-  Dot 

ShaderGraph Node

# Dot

A pass-through node used for visually routing edges in the graph.

## Parameter Types

- Dot (float)
- Dot (half)
- Dot (integer)
- Dot (string)
- Dot (imageFile)
- Dot (vector4f)
- Dot (Surface Shader)
- Dot (vector2f)
- Dot (matrix4x4f)
- Dot (color3f)
- Dot (bool)
- Dot (matrix3x3f)
- Dot (vector3f)
- Dot (color4f)

| Input  | Type   |
|--------|--------|
| `In`   | Float  |
| `Note` | String |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input  | Type   |
|--------|--------|
| `In`   | Half   |
| `Note` | String |

| Output | Type |
|--------|------|
| `Out`  | Half |

| Input  | Type   |
|--------|--------|
| `In`   | Int32  |
| `Note` | String |

| Output | Type  |
|--------|-------|
| `Out`  | Int32 |

| Input  | Type   |
|--------|--------|
| `In`   | String |
| `Note` | String |

| Output | Type   |
|--------|--------|
| `Out`  | String |

| Input  | Type      |
|--------|-----------|
| `In`   | AssetPath |
| `Note` | String    |

| Output | Type      |
|--------|-----------|
| `Out`  | AssetPath |

| Input  | Type     |
|--------|----------|
| `In`   | Vector4f |
| `Note` | String   |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input  | Type   |
|--------|--------|
| `In`   | Token  |
| `Note` | String |

| Output | Type  |
|--------|-------|
| `Out`  | Token |

| Input  | Type     |
|--------|----------|
| `In`   | Vector2f |
| `Note` | String   |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input  | Type       |
|--------|------------|
| `In`   | Matrix4x4f |
| `Note` | String     |

| Output | Type       |
|--------|------------|
| `Out`  | Matrix4x4f |

| Input  | Type   |
|--------|--------|
| `In`   | Color3 |
| `Note` | String |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input  | Type   |
|--------|--------|
| `In`   | Bool   |
| `Note` | String |

| Output | Type |
|--------|------|
| `Out`  | Bool |

| Input  | Type       |
|--------|------------|
| `In`   | Matrix3x3f |
| `Note` | String     |

| Output | Type       |
|--------|------------|
| `Out`  | Matrix3x3f |

| Input  | Type     |
|--------|----------|
| `In`   | Vector3f |
| `Note` | String   |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input  | Type   |
|--------|--------|
| `In`   | Color4 |
| `Note` | String |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

## Dicussion

The Dot node is only visual; it has no effect on its input or output. Use the Dot node to make a graph more readable and visually appealing.

