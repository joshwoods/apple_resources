

- ShaderGraph
- 2D-Procedural
-  Worley Noise 2D 

ShaderGraph Node

# Worley Noise 2D

A 2D Worley noise generator.

## Parameter Types

- Worley Noise 2D (float)
- Worley Noise 2D (vector3f)
- Worley Noise 2D (vector2f)

| Input                 | Type     |
|-----------------------|----------|
| `Texture Coordinates` | Vector2f |
| `Jitter`              | Float    |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input                 | Type     |
|-----------------------|----------|
| `Texture Coordinates` | Vector2f |
| `Jitter`              | Float    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input                 | Type     |
|-----------------------|----------|
| `Texture Coordinates` | Vector2f |
| `Jitter`              | Float    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

## Parameter description

`Texture Coordinates`  
The 2D coordinate at which the data is read in order to map the texture onto a surface. The default uses the current *UV* coordinates, in which *U* is the horizontal axis and *V* is the vertical axis.

`Jitter`  
The amount to *jitter* or shift the center of each cell experiences. The default value is `1.0`. A smaller value creates a more regular pattern, and `0` creates perfect squares.

## Discussion

The Worley Noise 2D node procedurally generates nonuniform cellular regions. A finite number of center points are created, and each region is a polygon that surrounds the points closest to each center point. Below is an example of a simple node graph that uses the Worley Noise 2D Node to generate a black and white pattern procedurally.

Multiply the incoming texture coordinates with a constant float, which changes the frequency of the generated noise. A higher value coresponds to the pattern repeating more often. You then run the output through a convert node to change it to a black and white color value.  
Below, the resulting texture applies to a cube.

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

Cellular Noise 2D

A 2D cellular noise generator.

