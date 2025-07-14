

- ShaderGraph
- Compositing
-  Unpremultiply 

ShaderGraph Node

# Unpremultiply

Divides the RGB channels of the input by the alpha channel.

## Parameter Types

| Input | Type   |
|-------|--------|
| `In`  | Color4 |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

## See Also

### Nodes

Premultiply

Multiplies the RGB channels of the input by the alpha channel.

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

Inside

Multiplies a mask to all channels of the input.

