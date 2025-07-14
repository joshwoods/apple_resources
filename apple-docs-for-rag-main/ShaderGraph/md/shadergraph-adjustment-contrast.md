

- ShaderGraph
- Adjustment
-  Contrast 

ShaderGraph Node

# Contrast

Increases or decreases contrast of values using a linear slope multiplier.

## Parameter Types

- Contrast (float)
- Contrast (vector3f FA)
- Contrast (vector4f)
- Contrast (vector4f FA)
- Contrast (color3f FA)
- Contrast (color4f FA)
- Contrast (vector2f FA)
- Contrast (vector3f)
- Contrast (color4f)
- Contrast (vector2f)
- Contrast (color3f)

| Input    | Type  |
|----------|-------|
| `In`     | Float |
| `Amount` | Float |
| `Pivot`  | Float |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input    | Type     |
|----------|----------|
| `In`     | Vector3f |
| `Amount` | Float    |
| `Pivot`  | Float    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input    | Type     |
|----------|----------|
| `In`     | Vector4f |
| `Amount` | Vector4f |
| `Pivot`  | Vector4f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input    | Type     |
|----------|----------|
| `In`     | Vector4f |
| `Amount` | Float    |
| `Pivot`  | Float    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input    | Type   |
|----------|--------|
| `In`     | Color3 |
| `Amount` | Float  |
| `Pivot`  | Float  |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input    | Type   |
|----------|--------|
| `In`     | Color4 |
| `Amount` | Float  |
| `Pivot`  | Float  |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input    | Type     |
|----------|----------|
| `In`     | Vector2f |
| `Amount` | Float    |
| `Pivot`  | Float    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input    | Type     |
|----------|----------|
| `In`     | Vector3f |
| `Amount` | Vector3f |
| `Pivot`  | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input    | Type   |
|----------|--------|
| `In`     | Color4 |
| `Amount` | Color4 |
| `Pivot`  | Color4 |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input    | Type     |
|----------|----------|
| `In`     | Vector2f |
| `Amount` | Vector2f |
| `Pivot`  | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input    | Type   |
|----------|--------|
| `In`     | Color3 |
| `Amount` | Color3 |
| `Pivot`  | Color3 |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

## Parameter descriptions

`In`  
The input value to modify.

`Amount`  
The linear slope multiplier that increases or decreases the contrast. A value between `0.0` and `1.0` decreases the contrast of the `In` parameter, while a value greater than `1.0` increases it.

`Pivot`  
The center value of the contrast adjustment. As contrast increases, values of the `In` parameter get further away from this value. As contrast decreases, values of the `In` parameter get closer to this value.

## Discussion

Below is an example of a simple node graph that uses the the Contrast node to make a black and white arrow texture more gray and closer in color.

Below, the resulting texture applies to a cube.

In this contrast node, the value of the `Pivot` input is `0.2`, which represents a dark gray. The value of the `Amount` input is also `0.2`, indicating that the contrast of the input decreases and the color value of our texture gets closer to the `Pivot` input. As a result, the output texture of the node becomes a gray version of the original black and white arrow texture.

## See Also

### Nodes

Remap

Linearly remaps incoming values from one range to another.

Smooth Step

Outputs a smooth remapping from low-high to 0-1.

Luminance

Outputs a grayscale value containing the luminance of the incoming RGB color in all color channels.

RGB to HSV

Converts a color from RGB to HSV space.

HSV to RGB

Converts a color from HSV to RGB space.

Range

Remaps incoming values from one range to another.

HSV Adjust

Adjusts the hue, saturation and value of an RGB color by a vector .

Saturate

Adjusts the saturation of a color.

Step (RealityKit)

Outputs a 1 or a 0 depending on whether the input is greater than or less than the edge value.

