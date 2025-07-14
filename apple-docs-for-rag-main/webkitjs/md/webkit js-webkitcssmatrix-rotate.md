

- WebKit JS
- WebKitCSSMatrix
-  rotate 

Instance Method

# rotate

Returns the result of rotating this matrix by a given vector.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
WebKitCSSMatrix rotate(
    optional unrestricted double rotX, 
    optional unrestricted double rotY, 
    optional unrestricted double rotZ
);
```

## Parameters 

`rotX`  

The x component in the vector, in degrees.

`rotY`  

The y component in the vector, in degrees. If undefined, the x component is used.

`rotZ`  

The z component in the vector, in degrees. If undefined, the x component is used.

## Return Value

A new matrix that is the result of rotating this matrix by each of the three rotation matrices about the major axes, first the x axes, y axes, and then z axes.

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

rotateAxisAngle

Returns the result of rotating this matrix by a given vector and angle.

skewX

Specifies a skew transformation along the x-axis by the given angle.

skewY

Specifies a skew transformation along the y-axis by the given angle.

