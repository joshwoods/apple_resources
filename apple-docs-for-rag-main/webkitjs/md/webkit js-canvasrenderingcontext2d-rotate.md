

- WebKit JS
- CanvasRenderingContext2D
-  rotate 

Instance Method

# rotate

Rotates the canvas coordinate system.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
void rotate(
    unrestricted float angle
);
```

## Parameters 

`angle`  

The amount of rotation, in radians, clockwise.

## Discussion

Changes to the coordinate system affect subsequent drawing operations, but do not affect anything already drawn. Rotation is clockwise around the origin, which by default is the upper-left corner.

## See Also

### Changing the Coordinate System

scale

Scales the canvas coordinate system horizontally and vertically.

setTransform

Sets the transformation matrix.

transform

Transforms the current transformation matrix using another matrix.

translate

Moves the origin of the canvas coordinate system.

