

- ShaderGraph
- Geometric
-  Geometric Property 

ShaderGraph Node

# Geometric Property

The value of the specified geometric property (defined using ) of the currently-bound geometry.

## Parameter Types

- Geometric Property (float)
- Geometric Property (color4f)
- Geometric Property (vector2f)
- Geometric Property (vector3f)
- Geometric Property (color3f)

| Input      | Type   |
|------------|--------|
| `Geomprop` | String |
| `Default`  | Float  |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input      | Type   |
|------------|--------|
| `Geomprop` | String |
| `Default`  | Color4 |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input      | Type     |
|------------|----------|
| `Geomprop` | String   |
| `Default`  | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input      | Type     |
|------------|----------|
| `Geomprop` | String   |
| `Default`  | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input      | Type   |
|------------|--------|
| `Geomprop` | String |
| `Default`  | Color3 |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

## Parameter descriptions

`Geomprop`  
The name of the geometric property to be read.

`Default`  
The value the node returns if it’s unable to read the geometric property.

## Discussion

The Geometric Property node attempts to return the value of the geometric property with the name defined by the `Geomprop` parameter. If that property doesn’t exist or there’s an error retrieving the property’s value, the node outputs the value of the `Default` parameter.

Note

The type of this node must be the same as the type of the geometric property you’re attempting to reference.

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

Reflect (RealityKit)

Reflects a vector about another vector.

Refract (RealityKit)

Refracts a vector using a given normal and index of refraction (eta).

