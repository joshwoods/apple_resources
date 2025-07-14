

- ShaderGraph
- Adjustment
-  Luminance 

ShaderGraph Node

# Luminance

Outputs a grayscale value containing the luminance of the incoming RGB color in all color channels.

## Parameter Types

- Luminance (color3f)
- Luminance (color4f)

| Input               | Type   |
|---------------------|--------|
| `In`                | Color3 |
| `Luma Coefficients` | Color3 |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input               | Type   |
|---------------------|--------|
| `In`                | Color4 |
| `Luma Coefficients` | Color3 |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

## Parameter descriptions

`In`  
The input to convert to grayscale.

`Luma Coefficients`  
The luma coefficients of the color space. The possible values for this node are the luma coeffiecients for the color spaces `acescg`, `rec202/rec2100`, or `rec709`. The default value is the luma coeffiecients for `acescg`, which are `(0.2722287, 0.6740818, 0.0536895)`.

## Discussion

The Luminance node takes in a color input and outputs that input as a grayscale image. The node computes the grayscale of an image by taking the dot product of the luma coefficients and the color vector. Below is an example of a simple node graph that uses the luminance node to convert an image to grayscale.

Below, the resulting texture applies to a cube.

## See Also

### Nodes

Remap

Linearly remaps incoming values from one range to another.

Smooth Step

Outputs a smooth remapping from low-high to 0-1.

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

Saturate

Adjusts the saturation of a color.

Step (RealityKit)

Outputs a 1 or a 0 depending on whether the input is greater than or less than the edge value.

