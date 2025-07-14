

- WebKit JS
- WebKitCSSMatrix
-  rotateAxisAngle 

Instance Method

# rotateAxisAngle

Returns the result of rotating this matrix by a given vector and angle.

Safari Desktop 4.0+Safari Mobile 2.0+

``` source
WebKitCSSMatrix rotateAxisAngle(
    optional unrestricted double x, 
    optional unrestricted double y, 
    optional unrestricted double z, 
    optional unrestricted double angle
);
```

## Parameters 

`x`  

The x component in the vector, in degrees.

`y`  

The y component in the vector, in degrees. If undefined, the x component is used.

`z`  

The z component in the vector, in degrees. If undefined, the x component is used.

`angle`  

The angle of rotation about the axis vector, in degrees.

## Return Value

A new matrix that is the result of rotating this matrix by each of the three rotation matrices about the major axes and angle. The right-hand rule is used to determine the direction of rotation.

## Discussion

This matrix is not modified by this method.

## See Also

### Applying Operations

multiply

Returns the result of multiplying this matrix by a given matrix that is on the right.

inverse

Returns the inverse of this matrix.

translate

Returns the result of translating this matrix by a given vector.

scale

Returns the result of scaling this matrix by a given vector.

rotate

Returns the result of rotating this matrix by a given vector.

skewX

Specifies a skew transformation along the x-axis by the given angle.

skewY

Specifies a skew transformation along the y-axis by the given angle.

