

- WebKit JS
- WebKitCSSMatrix
-  setMatrixValue 

Instance Method

# setMatrixValue

Sets the matrix values using a string representation.

Safari Desktop 4.0+Safari Mobile 2.0+

``` source
void setMatrixValue(
    optional DOMString string
);
```

## Parameters 

`string`  

A string returned by the matrix3d transform function—typically returned by `window.getComputedStyle(element).webkitTransform()`.

