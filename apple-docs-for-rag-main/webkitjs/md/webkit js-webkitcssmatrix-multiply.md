

- WebKit JS
- WebKitCSSMatrix
-  multiply 

Instance Method

# multiply

Returns the result of multiplying this matrix by a given matrix that is on the right.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
WebKitCSSMatrix multiply(
    optional WebKitCSSMatrix? secondMatrix
);
```

## Parameters 

`secondMatrix`  

The matrix to multiply.

## Return Value

A new matrix that is the result of multiplying this matrix by the given matrix.

## Discussion

The given matrix is on the right of the multiplication. This matrix is not modified by this method.

## See Also

### Applying Operations

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

skewY

Specifies a skew transformation along the y-axis by the given angle.

