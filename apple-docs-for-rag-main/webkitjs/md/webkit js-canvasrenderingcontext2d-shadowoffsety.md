

- WebKit JS
- CanvasRenderingContext2D
-  shadowOffsetY 

Instance Property

# shadowOffsetY

A floating-point number that controls the vertical offset of shadows from the elements casting the shadows.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute unrestricted float shadowOffsetY;
```

## Discussion

Shadows are cast `shadowOffsetY` pixels down, regardless of the canvas rotation, scale, or transformation. If `shadowOffsetY` is negative, shadows are cast up.

Shadows are cast if `shadowOffsetY` is nonzero and the alpha value of `shadowColor` is nonzero.

## See Also

### Working with Shadows

clearShadow

Turns shadows off.

shadowBlur

A floating-point number that controls the degree of Gaussian blur applied to shadows.

shadowColor

A string that contains the RGBa color value of shadows.

shadowOffsetX

A floating-point number that controls the horizontal offset of shadows from the elements casting the shadows.

