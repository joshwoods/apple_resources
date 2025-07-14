

- ShaderGraph
- Math
-  Place 2D 

ShaderGraph Node

# Place 2D

Transforms UV texture coordinates for 2D texture placement.

## Parameter Types

| Input                 | Type     |
|-----------------------|----------|
| `Texture Coordinates` | Vector2f |
| `Pivot`               | Vector2f |
| `Scale`               | Vector2f |
| `Rotate`              | Float    |
| `Offset`              | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

## Parameter descriptions

`Texture Coordinates`  
The input texture coordinates to transform. The default value is the current surface texture coordinates with an index of `0`.

`Pivot`  
The pivot point for scaling and rotating the texture coordinates. The node subtracts this value from *U* and *V* before it applies the scale or rotation. The node then adds this value back later.

`Scale`  
The value by which to scale the texture coordinates. The node divides the *U* and *V* coordinates by this value. The default value is `(1,1)`

`Rotate`  
The number of degrees to rotate the texture coordinates. A postive value rotates the texture coordinates by that many degrees counter-clockwise and the resulting image clockwise. A negative value rotates the texture coordinates by that many degrees clockwise and the resulting image counter-clockwise. The default value is `0`.

`Offset`  
The value to offset the postion of the texture coordinates. The node subtracts this value from the texture coordinates after it has been scaled, rotated, and the pivot has been added back. The default value is `(0,0)`.

## Discussion

The Place 2D node can be used to transform texture coordinates and apply these basic transformations to textures. Below is an example of a simple node graph that uses the Place 2D Node to transform texture coordinates that are then passed to an image node.

The incoming texture coordinates are transformed in three ways. They are scaled down to half the size, rotated 180 degrees, and offset by 0.5 in both the *U* and *V* direction. For the scale and rotation, the pivot point is set to `(0.5, 0.5)`. Because texture coordinates generally range from `(0-1)` this means the scale and rotation are done from the center point of the image. Below is the original image and the texture with the transformation applied.

Original Image

Image after transformations

## See Also

### Nodes

Add

Adds two values.

Subtract

Subtracts two values.

Multiply

Multiplies two values.

Divide

Divides two values.

Modulo

Outputs the remaining fraction after dividing the input by a value and subtracting the integer portion.

Abs

Outputs the per-channel absolute value of the input.

Floor

Outputs the nearest integer value, per-channel, less than or equal to the incoming values.

Ceiling

Outputs the nearest integer value, per-channel, greater than or equal to the incoming values.

Power

Raises the incoming value to an exponent.

Sin

The sine of the incoming value in radians.

Cos

The cosine of the incoming value in radians.

Tan

The tangent of the incoming value in radians.

Asin

The arcsine of the incoming value in radians.

Acos

The arccosine of the incoming value in radians.

Atan2

The arctangent of the expression (iny/inx) in radians.

