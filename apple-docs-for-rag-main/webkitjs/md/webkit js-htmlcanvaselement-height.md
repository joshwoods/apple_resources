

- WebKit JS
- HTMLCanvasElement
-  height 

Instance Property

# height

An integer containing the height of the canvas in CSS pixels.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
attribute unsigned long height;
```

## Discussion

Setting the `width` or `height` property, even without changing it, clears the canvas to transparent black and resets all context settings to their defaults, including the coordinate system and transformation matrix. If the `height` attribute is not specified in the `` tag, the default height is 150 pixels.

## See Also

### Setting Canvas Dimensions

width

An integer containing the width of the canvas in CSS pixels.

