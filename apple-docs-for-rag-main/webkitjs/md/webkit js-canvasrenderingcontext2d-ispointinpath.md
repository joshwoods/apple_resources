

- WebKit JS
- CanvasRenderingContext2D
-  isPointInPath 

Instance Method

# isPointInPath

Determines whether a specified point is within the area defined by the current path.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
boolean isPointInPath(
    DOMPath path, 
    unrestricted float x, 
    unrestricted float y, 
    optional CanvasWindingRule winding
);
```

## Parameters 

`x`  

The x-coordinate of the point in the canvas coordinate system.

`y`  

The y-coordinate of the point in the canvas coordinate system.

## Return Value

Returns `true` if the point is within the path.

## Discussion

All parameter values are in the canvas’s current coordinate system, subject to the current transformation matrix (rotation, scale, and so on).

## See Also

### Creating Paths (Lines, Curves, Arcs, and Shapes)

beginPath

Denotes the beginning of new path.

clip

Constrains the clipping region of the canvas to the current path.

