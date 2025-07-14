

- WebKit JS
- CanvasRenderingContext2D
-  clearShadow 

Instance Method

# clearShadow

Turns shadows off.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
void clearShadow();
```

## Discussion

When you set a shadow color or shadow blur, and a shadow offset, all subsequent drawing operations include a shadow of the current color and blur, at the specified offset. The `clearShadow` method is a convenient way to turn shadows off.

Note

The `clearShadow()` method is not currently part of the HTML5 specification. It is supported in Safari and other Webkit-based browsers.

## See Also

### Working with Shadows

shadowBlur

A floating-point number that controls the degree of Gaussian blur applied to shadows.

shadowColor

A string that contains the RGBa color value of shadows.

shadowOffsetX

A floating-point number that controls the horizontal offset of shadows from the elements casting the shadows.

shadowOffsetY

A floating-point number that controls the vertical offset of shadows from the elements casting the shadows.

