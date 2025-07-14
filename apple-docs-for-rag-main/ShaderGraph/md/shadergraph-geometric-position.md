

- ShaderGraph
- Geometric
-  Position 

ShaderGraph Node

# Position

The coordinates of the currently-processed data in a given coordinate space.

## Parameter Types

| Input   | Type   |
|---------|--------|
| `Space` | String |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

## Parameter description

`Space`  
The space in which the shader defines the position vector. The valid spaces for this input are `model`, `object`, `tangent`, and `world`. The default value is `object`.

## See Also

### Nodes

Normal

The geometric normal of the currently-processed data in a given coordinate space.

Tangent

The geometric tangent of the currently-processed data in a given coordinate space.

Bitangent

The geometric bitangent vector of the currently-processed data in a given coordinate space.

Texture Coordinates

The 2D or 3D texture coordinates of the currently-processed data.

Geometry Color

The color associated with the geometry at the currently-processed geometric position, typically defined by vertex color.

Geometric Property

The value of the specified geometric property (defined using ) of the currently-bound geometry.

Reflect (RealityKit)

Reflects a vector about another vector.

Refract (RealityKit)

Refracts a vector using a given normal and index of refraction (eta).

