

- WebKit JS
- CanvasRenderingContext2D
-  translate 

Instance Method

# translate

Moves the origin of the canvas coordinate system.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
void translate(
    unrestricted float tx, 
    unrestricted float ty
);
```

## Parameters 

`tx`  

The x-coordinate in the current canvas coordinate system to be made the new origin.

`ty`  

The y-coordinate in the current canvas coordinate system to be made the new origin.

## Discussion

The specified point x,y in the canvas coordinate system becomes the point 0,0 and the entire coordinate system is translated accordingly.

## See Also

### Changing the Coordinate System

rotate

Rotates the canvas coordinate system.

scale

Scales the canvas coordinate system horizontally and vertically.

setTransform

Sets the transformation matrix.

transform

Transforms the current transformation matrix using another matrix.

