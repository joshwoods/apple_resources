

- ShaderGraph
- Compositing
-  Mix 

ShaderGraph Node

# Mix

Mixes foreground and background inputs, weighting based on mix value.

## Parameter Types

- Mix (float)
- Mix (vector4h)
- Mix (vector2f)
- Mix (color4f)
- Mix (vector3f)
- Mix (color3f)
- Mix (vector3h)
- Mix (vector4f)
- Mix (vector2h)
- Mix (half)

| Input        | Type  |
|--------------|-------|
| `Foreground` | Float |
| `Background` | Float |
| `Mix`        | Float |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input        | Type     |
|--------------|----------|
| `Foreground` | Vector4h |
| `Background` | Vector4h |
| `Mix`        | Float    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4h |

| Input        | Type     |
|--------------|----------|
| `Foreground` | Vector2f |
| `Background` | Vector2f |
| `Mix`        | Float    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input        | Type   |
|--------------|--------|
| `Foreground` | Color4 |
| `Background` | Color4 |
| `Mix`        | Float  |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input        | Type     |
|--------------|----------|
| `Foreground` | Vector3f |
| `Background` | Vector3f |
| `Mix`        | Float    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input        | Type   |
|--------------|--------|
| `Foreground` | Color3 |
| `Background` | Color3 |
| `Mix`        | Float  |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input        | Type     |
|--------------|----------|
| `Foreground` | Vector3h |
| `Background` | Vector3h |
| `Mix`        | Float    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3h |

| Input        | Type     |
|--------------|----------|
| `Foreground` | Vector4f |
| `Background` | Vector4f |
| `Mix`        | Float    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input        | Type     |
|--------------|----------|
| `Foreground` | Vector2h |
| `Background` | Vector2h |
| `Mix`        | Float    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2h |

| Input        | Type |
|--------------|------|
| `Foreground` | Half |
| `Background` | Half |
| `Mix`        | Half |

| Output | Type |
|--------|------|
| `Out`  | Half |

## Parameter descriptions

`Foreground`  
The foreground input.

`Background`  
The background input.

`Mix`  
The weight that determines what the output value is closer to. The default value is `0`. Values outside of the range `0-1` produce an undefined effect outside of the node’s intended function.

## Discussion

The Mix node blends two input values together, represented by the equation `F * m + B(1 - m)`. If the `Mix` value is `1`, the output is identical to the `Foreground` value. If the value is `0`, the output is identical to the `Background` value. The closer the `Mix` value is to `0` or `1`, the closer the output will be to the corresponding input. Use the Mix node to blend between two different textures and create transtions or effects, interpolate between two colors, or mix shader parameters. Below is an example of a simple node graph that uses the Mix node to blend two images together into a single material.

Below are the original two images and the resulting mixed texture applied to a cube with `Mix` values of `0.1`, `0.5`, and `0.9`.

Foreground

Background

Mix value of 0.1

Mix value of 0.5

Mix value of 0.9

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

