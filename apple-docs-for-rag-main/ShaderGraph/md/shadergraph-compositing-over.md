

- ShaderGraph
- Compositing
-  Over 

ShaderGraph Node

# Over

A merge operation that layers foreground over background, using the alpha of the foreground.

## Parameter Types

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
The `color4` foreground input. `F` represents the RGB component of this parameter. `f` represents the alpha component of this parameter.

`Background`  
The `color4` background input. `B` represents the RGB component of this parameter. `b`represents the alpha component of this parameter.

`Mix`  
The weight of the blend operation. The higher the value of `Mix`, the more apparent the effect of the blend operation. The default value is `1`. Values outside of the range `0-1` produce an undefined effect outside of the node’s intended function.

## Discussion

The Over node determines its output using the alpha channels of the foreground and background inputs. The RGB component of the output is `F+B(1-f)` and the alpha component of the output is `f+b(1-f)`. The lower the alpha of the foreground, the more the background blends into the foreground. Below is a simple node graph that uses the Over node to blend a wood and rock texture.

Below are the two original images, the image representation of the alpha of the foreground, and the resulting blended texture applied to a cube.

Foreground

Foreground Alpha

Background

Blended texture

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

Inside

Multiplies a mask to all channels of the input.

