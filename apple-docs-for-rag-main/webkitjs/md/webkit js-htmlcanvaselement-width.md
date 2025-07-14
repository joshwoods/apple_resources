

- WebKit JS
- HTMLCanvasElement
-  width 

Instance Property

# width

An integer containing the width of the canvas in CSS pixels.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
attribute unsigned long width;
```

## Discussion

Setting the `width` or `height` property, even without changing it, clears the canvas to transparent black and resets all context settings to their defaults, including the coordinate system and transformation matrix. If the `width` attribute is not specified in the `` tag, the default width is 300 pixels.

## See Also

### Setting Canvas Dimensions

height

An integer containing the height of the canvas in CSS pixels.

