

- ShaderGraph
- 2D-Procedural
-  Cellular Noise 2D 

ShaderGraph Node

# Cellular Noise 2D

A 2D cellular noise generator.

## Parameter Types

| Input                 | Type     |
|-----------------------|----------|
| `Texture Coordinates` | Vector2f |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

## Parameter descriptions

`Texture Coordinates`  
The 2D coordinate at which the data is read in order to map the texture onto a surface. The default is to use the current *UV* coordinates, in which *U* is the horizontal axis and *V* is the vertical axis.

## Discussion

The Cellular Noise 2D shader node procedurally generates noise patterns that can be used to add texture and variation to materials. Below is an example of a simple node graph that uses the Cellular Noise 2D Node to generate a black and white pattern procedurally.

Multiply the incoming texture coordinates with a constant float. The float changes the frequency of the generated noise to a higher number that corresponds with the pattern repeating more often. The output of the node runs through a convert node in order to change the float output to a black and white color output. Below, the resulting texture applies to a cube.

## See Also

### Nodes

Ramp Horizontal

A left-to-right linear value ramp (gradient) generator.

Ramp Vertical

A top-to-bottom linear value ramp (gradient) generator.

Ramp 4 Corners

A four-point linear value ramp (gradient) generator.

Split Horizontal

A left-to-right split matte, split at a specified U value.

Split Vertical

A top-to-bottom split matte, split at a specified V value.

Noise 2D

A 2D Perlin noise generator.

Worley Noise 2D

A 2D Worley noise generator.

