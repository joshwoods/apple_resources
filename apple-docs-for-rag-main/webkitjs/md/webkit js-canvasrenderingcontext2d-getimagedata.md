

- WebKit JS
- CanvasRenderingContext2D
-  getImageData 

Instance Method

# getImageData

Gets an `imageData` object containing an RGBa pixel array corresponding to a rectangular area of the canvas.

Safari Desktop 4.0+Safari Mobile 3.0+

``` source
ImageData getImageData(
    float sx, 
    float sy, 
    float sw, 
    float sh
);
```

## Parameters 

`sx`  

The x-coordinate of the left edge of the rectangle.

`sy`  

The y-coordinate of the top of the rectangle.

`sw`  

The width of the rectangle.

`sh`  

The height of the rectangle.

## Return Value

An `imageData` object.

## Discussion

All parameter values are in pixels relative to the upper-left corner of the canvas, *not* the current canvas coordinate system. The returned `imageData` object has two read-only properties: `width` and `height`. The `imageData` object’s `data` property is a one-dimensional array of RGBa pixel values in row order from left to right, with four values for each pixel—red, green, blue, and alpha. The RGBa values are integers with a range of 0-255, inclusive.

## See Also

### Manipulating Pixels

createImageData

Creates an opaque object whose `data` property contains a one-dimensional array of pixel values, initialized to transparent black.

putImageData

Blits the contents of an `imageData` object to the canvas. Alternatively, blits a specified region of the `imageData` object to the canvas.

