

- WebKit JS
- CanvasRenderingContext2D
-  globalAlpha 

Instance Property

# globalAlpha

A floating-point number controlling the degree of opacity for all drawing operations.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute unrestricted float globalAlpha;
```

## Discussion

Set the `globalAlpha` to any value between 0 and 1, inclusive, to set the degree of opacity for all subsequent drawing operations, with 0 being completely transparent and 1 being completely opaque. Any pixels drawn subsequently have their alpha channel value multiplied by the `globalAlpha` value.

## See Also

### Compositing

globalCompositeOperation

A string representing the compositing method for drawing operations.

