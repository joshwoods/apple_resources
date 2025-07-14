

- WebKit JS
- CanvasRenderingContext2D
-  strokeRect 

Instance Method

# strokeRect

Draws a rectangle using the current stroke color, pattern, or gradient.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
void strokeRect(
    unrestricted float x, 
    unrestricted float y, 
    unrestricted float width, 
    unrestricted float height
);
```

## Parameters 

`x`  

The left edge of the rectangle, in units right from the origin of the canvas coordinate system.

`y`  

The top of the rectangle, in units down from the origin of the canvas coordinate system.

`width`  

The width of the rectangle, in canvas coordinate units.

`height`  

The height of the rectangle, in canvas coordinate units.

## Discussion

All parameter values are in the canvas’s current coordinate system, subject to the current transformation matrix (rotation, scale, and so on).

## See Also

### Drawing Rectangles

clearRect

Clears the specified rectangle to transparent black—RGBa(0,0,0,0).

fillRect

Fills a specified rectangle in the current fill color, gradient, or pattern.

