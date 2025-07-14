

- ShaderGraph
- Compositing
-  Burn 

ShaderGraph Node

# Burn

A blend operation that darkens the foreground layer using the background.

## Parameter Types

- Burn (float)
- Burn (half)
- Burn (color3f)
- Burn (color4f)

| Input        | Type  |
|--------------|-------|
| `Foreground` | Float |
| `Background` | Float |
| `Mix`        | Float |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

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
| `Foreground` | Color3 |
| `Background` | Color3 |
| `Mix`        | Float  |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

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
The weight of the blend effect. The higher the `Mix`, the greater the intensity of the blend operation, and the more the effect is visually apparent. The default value is `1`. Values outside of the range `0-1` produce an undefined effect outside of the node’s intended function.

## Discussion

The Burn node darkens each area in the background based on the darkness of the corresponding area in the foreground, represented by the equation `1 - (1 - B) / F`. Below is an example of a simple node graph that uses the the burn node to darken a brick texture.

Use a Noise 2D node to generate Perlin noise, and use the output of that texture as the foreground in the burn node. This process darkens the background brick texture according to the procedural pattern. Below, the resulting texture applies to a cube.

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

Inside

Multiplies a mask to all channels of the input.

