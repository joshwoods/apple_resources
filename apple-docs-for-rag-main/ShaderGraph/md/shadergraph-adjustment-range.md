

- ShaderGraph
- Adjustment
-  Range 

ShaderGraph Node

# Range

Remaps incoming values from one range to another.

## Parameter Types

- Range (float)
- Range (color3f)
- Range (color4f FA)
- Range (vector2f)
- Range (color4f)
- Range (vector3f FA)
- Range (vector4f FA)
- Range (color3f FA)
- Range (vector3f)
- Range (vector2f FA)
- Range (vector4f)

| Input      | Type  |
|------------|-------|
| `In`       | Float |
| `In Low`   | Float |
| `In High`  | Float |
| `Gamma`    | Float |
| `Out Low`  | Float |
| `Out High` | Float |
| `Do Clamp` | Bool  |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input      | Type   |
|------------|--------|
| `In`       | Color3 |
| `In Low`   | Color3 |
| `In High`  | Color3 |
| `Gamma`    | Color3 |
| `Out Low`  | Color3 |
| `Out High` | Color3 |
| `Do Clamp` | Bool   |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input      | Type   |
|------------|--------|
| `In`       | Color4 |
| `In Low`   | Float  |
| `In High`  | Float  |
| `Gamma`    | Float  |
| `Out Low`  | Float  |
| `Out High` | Float  |
| `Do Clamp` | Bool   |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input      | Type     |
|------------|----------|
| `In`       | Vector2f |
| `In Low`   | Vector2f |
| `In High`  | Vector2f |
| `Gamma`    | Vector2f |
| `Out Low`  | Vector2f |
| `Out High` | Vector2f |
| `Do Clamp` | Bool     |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input      | Type   |
|------------|--------|
| `In`       | Color4 |
| `In Low`   | Color4 |
| `In High`  | Color4 |
| `Gamma`    | Color4 |
| `Out Low`  | Color4 |
| `Out High` | Color4 |
| `Do Clamp` | Bool   |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input      | Type     |
|------------|----------|
| `In`       | Vector3f |
| `In Low`   | Float    |
| `In High`  | Float    |
| `Gamma`    | Float    |
| `Out Low`  | Float    |
| `Out High` | Float    |
| `Do Clamp` | Bool     |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input      | Type     |
|------------|----------|
| `In`       | Vector4f |
| `In Low`   | Float    |
| `In High`  | Float    |
| `Gamma`    | Float    |
| `Out Low`  | Float    |
| `Out High` | Float    |
| `Do Clamp` | Bool     |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input      | Type   |
|------------|--------|
| `In`       | Color3 |
| `In Low`   | Float  |
| `In High`  | Float  |
| `Gamma`    | Float  |
| `Out Low`  | Float  |
| `Out High` | Float  |
| `Do Clamp` | Bool   |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input      | Type     |
|------------|----------|
| `In`       | Vector3f |
| `In Low`   | Vector3f |
| `In High`  | Vector3f |
| `Gamma`    | Vector3f |
| `Out Low`  | Vector3f |
| `Out High` | Vector3f |
| `Do Clamp` | Bool     |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input      | Type     |
|------------|----------|
| `In`       | Vector2f |
| `In Low`   | Float    |
| `In High`  | Float    |
| `Gamma`    | Float    |
| `Out Low`  | Float    |
| `Out High` | Float    |
| `Do Clamp` | Bool     |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input      | Type     |
|------------|----------|
| `In`       | Vector4f |
| `In Low`   | Vector4f |
| `In High`  | Vector4f |
| `Gamma`    | Vector4f |
| `Out Low`  | Vector4f |
| `Out High` | Vector4f |
| `Do Clamp` | Bool     |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

## Parameter descriptions

`In`  
The input value to be remapped.

`In Low`  
The low end value of the input range. The default value is `0.0`.

`In High`  
The high end value of the input range. The default value is `1.0`.

`Gamma`  
The inverse exponent to apply to the input value. The inverse exponent is applied after first mapping the input range to the range `0..1`. The default value is `1.0`.

`Out Low`  
The low end value of the output range. The default value is `0.0`.

`Out High`  
The high end value of the output range. The default value is `1.0`.

`Do Clamp`  
The Boolean value that indicates if the output is clamped. If true, the output clamps to the range defined by the `Out Low` and `Out High` parameters. The default value is `False`.

## Discussion

The Range node takes a range of incoming values and converts them to another range. The node also provides the option to apply a gamma correction, which occurs in the middle of the transformation process. The gamma value is the inverse exponent the node applies to the incoming values. For example, a value of `2` raises the incoming values to the power of `1/2`, effectively calculating the square root. The node also provides the option to clamp the output, which means any values below the `Out Low` parameter will be set to the value of `Out Low` and any values above the `Out High` parameter will be set to value of `Out High`.

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

Contrast

Increases or decreases contrast of values using a linear slope multiplier.

HSV Adjust

Adjusts the hue, saturation and value of an RGB color by a vector .

Saturate

Adjusts the saturation of a color.

Step (RealityKit)

Outputs a 1 or a 0 depending on whether the input is greater than or less than the edge value.

