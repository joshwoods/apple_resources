

- ShaderGraph
- Geometric
-  Reflect (RealityKit) 

ShaderGraph Node

# Reflect (RealityKit)

Reflects a vector about another vector.

## Parameter Types

| Input    | Type     |
|----------|----------|
| `In`     | Vector3f |
| `Normal` | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

## Parameter descriptions

`In`  
The input vector to be reflected.

`Normal`  
The vector that the `In` vector will be reflected with reference to.

## Discussion

The Reflect node reflects the `In` vector by taking into account the surface orientation determined by the `Normal` vector. The Reflect node first normalizes the `Normal` vector and then calculates the reflection direction using the formula `In - 2 * dot(Normal, In) * Normal`. In this equation, `dot()` represents the dot product of the two vectors.

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

Geometry Color

The color associated with the geometry at the currently-processed geometric position, typically defined by vertex color.

Geometric Property

The value of the specified geometric property (defined using ) of the currently-bound geometry.

Refract (RealityKit)

Refracts a vector using a given normal and index of refraction (eta).

