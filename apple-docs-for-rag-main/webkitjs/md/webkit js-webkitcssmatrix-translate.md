

- WebKit JS
- WebKitCSSMatrix
-  translate 

Instance Method

# translate

Returns the result of translating this matrix by a given vector.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
WebKitCSSMatrix translate(
    optional unrestricted double x, 
    optional unrestricted double y, 
    optional unrestricted double z
);
```

## Parameters 

`x`  

The x component in the vector.

`y`  

The y component in the vector.

`z`  

The z component in the vector. If undefined, `0` is used.

## Return Value

A new matrix that is the result of translating this matrix.

## Discussion

This matrix is not modified by this method.

## See Also

### Applying Operations

multiply

Returns the result of multiplying this matrix by a given matrix that is on the right.

inverse

Returns the inverse of this matrix.

scale

Returns the result of scaling this matrix by a given vector.

rotate

Returns the result of rotating this matrix by a given vector.

rotateAxisAngle

Returns the result of rotating this matrix by a given vector and angle.

skewX

Specifies a skew transformation along the x-axis by the given angle.

skewY

Specifies a skew transformation along the y-axis by the given angle.

