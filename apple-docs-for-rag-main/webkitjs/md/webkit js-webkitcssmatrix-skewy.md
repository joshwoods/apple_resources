

- WebKit JS
- WebKitCSSMatrix
-  skewY 

Instance Method

# skewY

Specifies a skew transformation along the y-axis by the given angle.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
WebKitCSSMatrix skewY(
    optional unrestricted double angle
);
```

## Parameters 

`angle`  

The angle amount in degrees to skew.

## Return Value

A new matrix that is the result of skewing this matrix by the specified angle along the y-axis.

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

rotateAxisAngle

Returns the result of rotating this matrix by a given vector and angle.

skewX

Specifies a skew transformation along the x-axis by the given angle.

