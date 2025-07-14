

- ShaderGraph
- Compositing
-  Screen 

ShaderGraph Node

# Screen

A blend operation that lightens areas that are darker than white.

## Parameter Types

- Screen (float)
- Screen (color3f)
- Screen (half)
- Screen (color4f)

| Input        | Type  |
|--------------|-------|
| `Foreground` | Float |
| `Background` | Float |
| `Mix`        | Float |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input        | Type   |
|--------------|--------|
| `Foreground` | Color3 |
| `Background` | Color3 |
| `Mix`        | Float  |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input        | Type |
|--------------|------|
| `Foreground` | Half |
| `Background` | Half |
| `Mix`        | Half |

| Output | Type |
|--------|------|
| `Out`  | Half |

| Input        | Type   |
|--------------|--------|
| `Foreground` | Color4 |
| `Background` | Color4 |
| `Mix`        | Float  |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

## Parameter descriptions

`Foreground`  
The foreground input. Represented by `F` in the mathmatical equation.

`Background`  
The background input. Represented by `B` in the mathmatical equation.

`Mix`  
The weight of the blend operation. The higher the value of `Mix`, the more apparent the effect of the blend operation. The default value is `1`. Values outside of the range `0-1` produce an undefined effect outside of the node’s intended function.

## Discussion

The Screen node inverts the color values of both the foreground and background and multiplies those values together. Then the node inverts the colors again. This is represented by the equation `1 - (1 - F)(1 - B)`. The resulting visual effect is always equally bright or brighter than the original textures. Below is an example of a simple node graph that uses the Screen node to blend two images together into a single material.

Below are two images and their resulting blended texture applied to a cube.

Foreground

Background

## See Also

### Nodes

Premultiply

Multiplies the RGB channels of the input by the alpha channel.

Unpremultiply

Divides the RGB channels of the input by the alpha channel.

Additive Mix

Adds foreground and background values.

Subtractive Mix

Subtracts foreground from background values.

Difference

Outputs the distance between foreground and background values.

Burn

A blend operation that darkens the foreground layer using the background.

Dodge

A blend operation that lightens the background layer depending on the foreground.

Overlay

A blend operation that multiplies dark areas and screens light areas.

Disjoint Over

A merge operation that layers foreground over background color, but assumes no overlap in partially transparent areas covered by both.

In

Outputs areas of foreground that overlap with the alpha of background.

Mask

Outputs areas of background that overlap with the alpha of foreground.

Matte

A merge operation that layers premultiplied foreground over background.

Out

Outputs areas of foreground that do not overlap with background.

Over

A merge operation that layers foreground over background, using the alpha of the foreground.

Inside

Multiplies a mask to all channels of the input.

