

- ShaderGraph
- Adjustment
-  HSV Adjust 

ShaderGraph Node

# HSV Adjust

Adjusts the hue, saturation and value of an RGB color by a vector .

## Parameter Types

- HSV Adjust (color3f)
- HSV Adjust (color4f)

| Input    | Type     |
|----------|----------|
| `In`     | Color3   |
| `Amount` | Vector3f |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input    | Type     |
|----------|----------|
| `In`     | Color4   |
| `Amount` | Vector3f |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

## Parameter descriptions

`In`  
The input color the node adjusts.

`Amount`  
The adjustment of the HSV. The default value is `(0,1,1)`, which causes no change.

## Discussion

The HSV Adjust node adjusts the hue, saturation, and value of the color passed to the `In` parameter. The node performs this adjustment by adding the first value of the `Amount` vector to the hue, multiplying the saturation by the second value of the `Amount` vector, and multiplying that value by the third value of the `Amount` vector. When adjusting the hue, a positive value rotates the hue in the direction of red to green to blue. A value of 1 represents an entire rotation, and results in no change.

Note

This node never changes the alpha of a `color4`.

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

Range

Remaps incoming values from one range to another.

Saturate

Adjusts the saturation of a color.

Step (RealityKit)

Outputs a 1 or a 0 depending on whether the input is greater than or less than the edge value.

