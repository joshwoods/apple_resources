

- WebKit JS
- CanvasRenderingContext2D
-  globalCompositeOperation 

Instance Property

# globalCompositeOperation

A string representing the compositing method for drawing operations.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute DOMString globalCompositeOperation;
```

## Discussion

By default, drawings layer on top of one another in drawing order, with opaque areas obscuring existing layers and transparent or translucent areas being blended with existing layers according to their alpha value. Set the `globalCompositeOperation` property to one of the `globalCompositeOperation` constants to override the default compositing method. The allowed values are `source-atop`, `source-in`, `source-out`, `source-over`, `destination-atop`, `destination-in`, `destination-out`, `destination-over`, `lighter`, `copy`, and `xor`. See Global Compositing Operation Constants for details.

## See Also

### Compositing

globalAlpha

A floating-point number controlling the degree of opacity for all drawing operations.

