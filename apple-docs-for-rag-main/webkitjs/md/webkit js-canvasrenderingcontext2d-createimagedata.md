

- WebKit JS
- CanvasRenderingContext2D
-  createImageData 

Instance Method

# createImageData

Creates an opaque object whose `data` property contains a one-dimensional array of pixel values, initialized to transparent black.

Safari Desktop 4.0+Safari Mobile 3.0+

``` source
ImageData createImageData(
    ImageData? imagedata
);
```

## Parameters 

`sw`  

The width of the pixel array.

`sh`  

The height of the pixel array.

## Return Value

An `imageData` object.

## Discussion

This method is typically used to create additional pixel arrays that can be blitted to the canvas in a single operation. You can optionally pass in another `imageData` object as a parameter, instead of a width and height, to create a new `imageData` object with the same pixel dimensions as the specified object.

## See Also

### Manipulating Pixels

getImageData

Gets an `imageData` object containing an RGBa pixel array corresponding to a rectangular area of the canvas.

putImageData

Blits the contents of an `imageData` object to the canvas. Alternatively, blits a specified region of the `imageData` object to the canvas.

