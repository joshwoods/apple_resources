

- WebKit JS
- CanvasRenderingContext2D
-  setTransform 

Instance Method

# setTransform

Sets the transformation matrix.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
void setTransform(
    unrestricted float m11, 
    unrestricted float m12, 
    unrestricted float m21, 
    unrestricted float m22, 
    unrestricted float dx, 
    unrestricted float dy
);
```

## Parameters 

`m11`  

Column 1 row 1 matrix value (a).

`m12`  

Column 1 row 2 matrix value (b).

`m21`  

Column 2 row 1 matrix value (c).

`m22`  

Column 2 row 2 matrix value (d).

`dx`  

X scalar value (e).

`dy`  

Y scalar value (f).

## Discussion

Replaces the current transformation matrix with the matrix shown in Figure 1. Each point in the canvas coordinate system is multiplied by the transformation matrix.

Figure 1 The transformation matrix

## See Also

### Changing the Coordinate System

rotate

Rotates the canvas coordinate system.

scale

Scales the canvas coordinate system horizontally and vertically.

transform

Transforms the current transformation matrix using another matrix.

translate

Moves the origin of the canvas coordinate system.

