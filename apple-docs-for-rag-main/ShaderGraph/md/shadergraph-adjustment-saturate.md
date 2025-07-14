

- ShaderGraph
- Adjustment
-  Saturate 

ShaderGraph Node

# Saturate

Adjusts the saturation of a color.

## Parameter Types

- Saturate (color3f)
- Saturate (color4f)

| Input               | Type   |
|---------------------|--------|
| `In`                | Color3 |
| `Amount`            | Float  |
| `Luma Coefficients` | Color3 |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input               | Type   |
|---------------------|--------|
| `In`                | Color4 |
| `Amount`            | Float  |
| `Luma Coefficients` | Color3 |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

## Parameter descriptions

`In`  
The input color to adjust the saturation of.

`Amount`  
The multiplier to apply to the saturation. The default value is `1.0`.

`Luma Coefficients`  
The luma coefficients of the color space. The possible values for this node are the luma coeffiecients for the color spaces `acescg`, `rec202/rec2100`, or `rec709`. The default value is the luma coeffiecients for `acescg`, which are `(0.2722287, 0.6740818, 0.0536895)`.

## Discussion

The Saturate node performs a linear interpolation between the incoming color value and the luminance of the incoming color value. Setting the value of the `Amount` parameter to `0` adjusts the output to a grayscale of the input equal to the value that the Luminance would output.

Note

The effect of this node isn’t equivalent to adjusting saturation with the HSV Adjust node. The Saturate node takes into account a colorspace when processing its modifications.

Below is an example of a simple node graph that uses the Saturate node to modify the saturation of an image.

Below, the resulting texture applies to a cube.

Original Texture

Amount: 0.5

Amount: 2

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

HSV Adjust

Adjusts the hue, saturation and value of an RGB color by a vector .

Step (RealityKit)

Outputs a 1 or a 0 depending on whether the input is greater than or less than the edge value.

