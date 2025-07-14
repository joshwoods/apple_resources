

- WebKit JS
- CanvasRenderingContext2D
-  clearRect 

Instance Method

# clearRect

Clears the specified rectangle to transparent black—RGBa(0,0,0,0).

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
void clearRect(
    unrestricted float x, 
    unrestricted float y, 
    unrestricted float width, 
    unrestricted float height
);
```

## Parameters 

`x`  

The x-coordinate of the left edge of the rectangle, in pixels from the left edge of the canvas coordinate system.

`y`  

The y-coordinate of the top of the rectangle, in pixels from the top of the canvas coordinate system.

`width`  

The width of the rectangle, in pixels.

`height`  

The height of the rectangle, in pixels.

## Discussion

All parameter values are in the canvas’s current coordinate system, subject to the current transformation matrix.

## See Also

### Drawing Rectangles

fillRect

Fills a specified rectangle in the current fill color, gradient, or pattern.

strokeRect

Draws a rectangle using the current stroke color, pattern, or gradient.

