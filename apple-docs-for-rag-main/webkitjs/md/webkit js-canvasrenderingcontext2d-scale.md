

- WebKit JS
- CanvasRenderingContext2D
-  scale 

Instance Method

# scale

Scales the canvas coordinate system horizontally and vertically.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
void scale(
    unrestricted float sx, 
    unrestricted float sy
);
```

## Parameters 

`sx`  

The horizontal scalar.

`sy`  

The vertical scalar.

## Discussion

Drawing operations can be scaled up or down by setting the scale. All drawing operation x and y coordinates, widths and heights are multiplied by the scalars. The scalars must be nonzero, but may be negative (which reverses the sign of subsequent x and y coordinates.

## See Also

### Changing the Coordinate System

rotate

Rotates the canvas coordinate system.

setTransform

Sets the transformation matrix.

transform

Transforms the current transformation matrix using another matrix.

translate

Moves the origin of the canvas coordinate system.

