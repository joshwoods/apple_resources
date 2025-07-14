

- WebKit JS
- CanvasRenderingContext2D
-  shadowOffsetX 

Instance Property

# shadowOffsetX

A floating-point number that controls the horizontal offset of shadows from the elements casting the shadows.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
attribute unrestricted float shadowOffsetX;
```

## Discussion

Shadows are cast `shadowOffsetX` pixels to the right, regardless of the canvas rotation, scale, or transformation. If `shadowOffsetX` is negative, shadows are cast to the left.

Shadows are cast if `shadowOffsetX` is nonzero and the alpha value of `shadowColor` is nonzero.

## See Also

### Working with Shadows

clearShadow

Turns shadows off.

shadowBlur

A floating-point number that controls the degree of Gaussian blur applied to shadows.

shadowColor

A string that contains the RGBa color value of shadows.

shadowOffsetY

A floating-point number that controls the vertical offset of shadows from the elements casting the shadows.

