

- ShaderGraph
- Geometric
-  Texture Coordinates 

ShaderGraph Node

# Texture Coordinates

The 2D or 3D texture coordinates of the currently-processed data.

## Parameter Types

- Texture Coordinates (vector2f)
- Texture Coordinates (vector4f)

| Input   | Type  |
|---------|-------|
| `Index` | Int32 |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input   | Type  |
|---------|-------|
| `Index` | Int32 |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

## Parameter description

`Index`  
The index of the texture coordinates to be referenced. The default value is `0`.

## See Also

### Nodes

Position

The coordinates of the currently-processed data in a given coordinate space.

Normal

The geometric normal of the currently-processed data in a given coordinate space.

Tangent

The geometric tangent of the currently-processed data in a given coordinate space.

Bitangent

The geometric bitangent vector of the currently-processed data in a given coordinate space.

Geometry Color

The color associated with the geometry at the currently-processed geometric position, typically defined by vertex color.

Geometric Property

The value of the specified geometric property (defined using ) of the currently-bound geometry.

Reflect (RealityKit)

Reflects a vector about another vector.

Refract (RealityKit)

Refracts a vector using a given normal and index of refraction (eta).

