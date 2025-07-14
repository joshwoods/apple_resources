

- WebKit JS
- CanvasRenderingContext2D
-  shadowBlur 

Instance Property

# shadowBlur

A floating-point number that controls the degree of Gaussian blur applied to shadows.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
attribute unrestricted float shadowBlur;
```

## Discussion

If shadows are enabled, each shadow has a Gaussian blur applied to its alpha value, with a standard deviation of `shadowBlur`. The `shadowBlur` value must be a positive number, and may be zero.

Shadows are cast if the value of the `shadowBlur` property is nonzero and the alpha value of `shadowColor` is nonzero.

## See Also

### Working with Shadows

clearShadow

Turns shadows off.

shadowColor

A string that contains the RGBa color value of shadows.

shadowOffsetX

A floating-point number that controls the horizontal offset of shadows from the elements casting the shadows.

shadowOffsetY

A floating-point number that controls the vertical offset of shadows from the elements casting the shadows.

