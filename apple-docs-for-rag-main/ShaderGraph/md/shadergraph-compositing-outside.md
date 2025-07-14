

- ShaderGraph
- Compositing
-  Outside 

ShaderGraph Node

# Outside

Multiplies (1 - mask) to all channels of the input.

## Parameter Types

- Outside (float)
- Outside (color3f)
- Outside (color4f)
- Outside (half)

| Input  | Type  |
|--------|-------|
| `In`   | Float |
| `Mask` | Float |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input  | Type   |
|--------|--------|
| `In`   | Color3 |
| `Mask` | Float  |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input  | Type   |
|--------|--------|
| `In`   | Color4 |
| `Mask` | Float  |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input  | Type |
|--------|------|
| `In`   | Half |
| `Mask` | Half |

| Output | Type |
|--------|------|
| `Out`  | Half |

## Parameter descriptions

`In`  
The input value to which the mask applies.

`Mask`  
The value by which the input is multiplied.

## Discussion

Below is an example of a simple node graph that uses the Outside node to apply a mask to a brick texture.

Below, the resulting texture applies to a cube.

Mask

Input

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

Screen

A blend operation that lightens areas that are darker than white.

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

