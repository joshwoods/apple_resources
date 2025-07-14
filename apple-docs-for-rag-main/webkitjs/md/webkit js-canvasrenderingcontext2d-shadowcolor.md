

- WebKit JS
- CanvasRenderingContext2D
-  shadowColor 

Instance Property

# shadowColor

A string that contains the RGBa color value of shadows.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
attribute DOMString shadowColor;
```

## Discussion

The value may be any CSS color value. If the alpha value of `shadowColor` is nonzero, shadows are cast, provided that at least one of the three properties `shadowBlur`, `shadowOffsetX`, or `shadowOffsetY` is also nonzero.

## See Also

### Working with Shadows

clearShadow

Turns shadows off.

shadowBlur

A floating-point number that controls the degree of Gaussian blur applied to shadows.

shadowOffsetX

A floating-point number that controls the horizontal offset of shadows from the elements casting the shadows.

shadowOffsetY

A floating-point number that controls the vertical offset of shadows from the elements casting the shadows.

