

- ShaderGraph
- Geometric
-  Geometry Color 

ShaderGraph Node

# Geometry Color

The color associated with the geometry at the currently-processed geometric position, typically defined by vertex color.

## Parameter Types

- Geometry Color (float)
- Geometry Color (color3f)
- Geometry Color (color4f)

| Input   | Type  |
|---------|-------|
| `Index` | Int32 |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input   | Type  |
|---------|-------|
| `Index` | Int32 |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input   | Type  |
|---------|-------|
| `Index` | Int32 |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

## Parameter description

`Index`  
The index of the color the node references. The default value is `0`.

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

Texture Coordinates

The 2D or 3D texture coordinates of the currently-processed data.

Geometric Property

The value of the specified geometric property (defined using ) of the currently-bound geometry.

Reflect (RealityKit)

Reflects a vector about another vector.

Refract (RealityKit)

Refracts a vector using a given normal and index of refraction (eta).

