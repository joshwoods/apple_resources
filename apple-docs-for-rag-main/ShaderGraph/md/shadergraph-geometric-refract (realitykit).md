

- ShaderGraph
- Geometric
-  Refract (RealityKit) 

ShaderGraph Node

# Refract (RealityKit)

Refracts a vector using a given normal and index of refraction (eta).

## Parameter Types

| Input    | Type     |
|----------|----------|
| `In`     | Vector3f |
| `Normal` | Vector3f |
| `Eta`    | Float    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

## Parameter descriptions

`In`  
The vector to refract.

`Normal`  
The normal of the surface from which the `In` vector refracts.

`Eta`  
The index of refraction.

## Discussion

The Refract node takes an incident vector `In` and calculates the direction of refraction off a surface.

Note

The vectors passed as the `In` and `Normal` parameters must both already be normalized in order to get the desired output.

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

Reflect (RealityKit)

Reflects a vector about another vector.

