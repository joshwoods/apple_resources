

- ShaderGraph
- 3D-Procedural
-  Cellular Noise 3D 

ShaderGraph Node

# Cellular Noise 3D

A 3D cellular noise generator.

## Parameter Types

| Input      | Type     |
|------------|----------|
| `Position` | Vector3f |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

## Parameter descriptions

`Position`  
The 3D coordinates at which the data is read in order to map the texture onto a surface. The default is to use the current 3D object-space coordinates.

## Discussion

The Cellular Noise 3D shader node procedurally generates noise patterns that can be used to add texture and variation to materials. Because this node generates noise in 3D, the texture will not repeat in the Z direction, but rather continue as depth changes. Below is an example of a simple node graph that uses the Cellular Noise 3D Node to generate a black and white pattern procedurally.

Multiply the incoming position with a constant float. The float changes the frequency of the generated noise to a higher number that corresponds with the pattern repeating more often. The output of the node runs through a convert node in order to change the float output to a black and white color output. Below, the resulting texture applies to a cube.

## See Also

### Nodes

Noise 3D

A 3D Perlin noise generator.

Fractal Noise 3D

Zero-centered 3D fractal noise created by summing several octaves of 3D Perlin noise.

Worley Noise 3D

A 3D Worley noise generator.

