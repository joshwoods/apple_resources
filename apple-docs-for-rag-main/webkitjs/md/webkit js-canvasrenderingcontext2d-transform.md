

- WebKit JS
- CanvasRenderingContext2D
-  transform 

Instance Method

# transform

Transforms the current transformation matrix using another matrix.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
void transform(
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

X scalar (e).

`dy`  

Y Scalar (f).

## Discussion

This method replaces the current transformation matrix with the result of a matrix multiplication between the current transformation matrix and the specified transformation matrix shown in Figure 1.

Figure 1 The transformation matrix

## See Also

### Changing the Coordinate System

rotate

Rotates the canvas coordinate system.

scale

Scales the canvas coordinate system horizontally and vertically.

setTransform

Sets the transformation matrix.

translate

Moves the origin of the canvas coordinate system.

