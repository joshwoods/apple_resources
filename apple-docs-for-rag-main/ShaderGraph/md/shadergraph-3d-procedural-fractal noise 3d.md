

- ShaderGraph
- 3D-Procedural
-  Fractal Noise 3D 

ShaderGraph Node

# Fractal Noise 3D

Zero-centered 3D fractal noise created by summing several octaves of 3D Perlin noise.

## Parameter Types

- Fractal Noise 3D (float)
- Fractal Noise 3D (vector2f)
- Fractal Noise 3D (vector4f)
- Fractal Noise 3D (vector3f FA)
- Fractal Noise 3D (color4f)
- Fractal Noise 3D (vector3f)
- Fractal Noise 3D (color4f FA)
- Fractal Noise 3D (vector2f FA)
- Fractal Noise 3D (color3f)
- Fractal Noise 3D (color3f FA)
- Fractal Noise 3D (vector4f FA)

| Input        | Type     |
|--------------|----------|
| `Amplitude`  | Float    |
| `Octaves`    | Int32    |
| `Lacunarity` | Float    |
| `Diminish`   | Float    |
| `Position`   | Vector3f |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input        | Type     |
|--------------|----------|
| `Amplitude`  | Vector2f |
| `Octaves`    | Int32    |
| `Lacunarity` | Float    |
| `Diminish`   | Float    |
| `Position`   | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input        | Type     |
|--------------|----------|
| `Amplitude`  | Vector4f |
| `Octaves`    | Int32    |
| `Lacunarity` | Float    |
| `Diminish`   | Float    |
| `Position`   | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input        | Type     |
|--------------|----------|
| `Amplitude`  | Float    |
| `Octaves`    | Int32    |
| `Lacunarity` | Float    |
| `Diminish`   | Float    |
| `Position`   | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input        | Type     |
|--------------|----------|
| `Amplitude`  | Vector4f |
| `Octaves`    | Int32    |
| `Lacunarity` | Float    |
| `Diminish`   | Float    |
| `Position`   | Vector3f |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input        | Type     |
|--------------|----------|
| `Amplitude`  | Vector3f |
| `Octaves`    | Int32    |
| `Lacunarity` | Float    |
| `Diminish`   | Float    |
| `Position`   | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input        | Type     |
|--------------|----------|
| `Amplitude`  | Float    |
| `Octaves`    | Int32    |
| `Lacunarity` | Float    |
| `Diminish`   | Float    |
| `Position`   | Vector3f |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input        | Type     |
|--------------|----------|
| `Amplitude`  | Float    |
| `Octaves`    | Int32    |
| `Lacunarity` | Float    |
| `Diminish`   | Float    |
| `Position`   | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input        | Type     |
|--------------|----------|
| `Amplitude`  | Vector3f |
| `Octaves`    | Int32    |
| `Lacunarity` | Float    |
| `Diminish`   | Float    |
| `Position`   | Vector3f |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input        | Type     |
|--------------|----------|
| `Amplitude`  | Float    |
| `Octaves`    | Int32    |
| `Lacunarity` | Float    |
| `Diminish`   | Float    |
| `Position`   | Vector3f |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input        | Type     |
|--------------|----------|
| `Amplitude`  | Float    |
| `Octaves`    | Int32    |
| `Lacunarity` | Float    |
| `Diminish`   | Float    |
| `Position`   | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

## Parameter descriptions

`Amplitude`  
The intensity of the generated noise. The higher the amplitude, the more pronounced the variations of the noise pattern.

`Octaves`  
The number of layers of 3D Perlin noise that the node sums together. The default value is 3.

`Lacunarity`  
The exponential scale between each octave. This value determines how different each successive octave or layer of Perlin noise is from one another. The default value is `2.0`

`Diminish`  
The rate that the amplitude of each successive octave is decreased. Maintain the value for this parameter in the range of `0.0-1.0`. The default value is `0.5`.

`Position`  
The 3D coordinates at which the data is read in order to map the texture onto a surface. The default is to use the current 3D object-space coordinates.

## Discussion

The Fractal Noise node produces its output by summing up multiple layers or octaves of 3D Perlin noise. The more octaves in the fractal noise, the finer the detail of the noise. Each successive octave differs from the previous; the `Lacunarity` and `Diminish` parameters determine the difference. *Lacunarity* refers to the difference in frequency between each octavex. As this value increases, the resulting fractal noise becomes more uneven and less smooth. *Diminish* refers to how the amplitude changes between octaves. A value of `1` indicates no change to the amplitude. As the value decreases, the amplitude from octave to octave decreases more quickly. Below is an example of a simple node graph that uses the Fractal Noise 3D node to generate a black and white pattern procedurally.

Multiply the incoming position with a constant float. The float changes the frequency of the generated noise to a higher number that corresponds with the pattern repeating more often. Below, the resulting texture applies to a cube with various values for each parameter. All values are the default, unless specified under the image.

1 Octave

3 Octaves

5 Octaves

Lacunarity of 1

Lacunarity of 2

Lacunarity of 5

Diminish of 0.2

Diminish of 0.5

Diminish of 1

## See Also

### Nodes

Noise 3D

A 3D Perlin noise generator.

Cellular Noise 3D

A 3D cellular noise generator.

Worley Noise 3D

A 3D Worley noise generator.

