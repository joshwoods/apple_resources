

- WebKit JS
- CanvasRenderingContext2D
-  clip 

Instance Method

# clip

Constrains the clipping region of the canvas to the current path.

Safari Desktop 3.0+Safari Mobile 1.0+

``` source
void clip(
    DOMPath path, 
    optional CanvasWindingRule winding
);
```

## Discussion

Use this method to treat the current path as a mask for drawing operations. For example, if you call `drawImage()` subsequent to calling `clip()`, the image is clipped at the borders of the current path.

## See Also

### Creating Paths (Lines, Curves, Arcs, and Shapes)

beginPath

Denotes the beginning of new path.

isPointInPath

Determines whether a specified point is within the area defined by the current path.

