

- WebKit JS
- CanvasRenderingContext2D
-  beginPath 

Instance Method

# beginPath

Denotes the beginning of new path.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
void beginPath();
```

## Discussion

Any calls to `arcTo`, `bezierCurveTo`, `lineTo`, `moveTo`, or `quadraticCurveTo` after a call to `beginPath` add elements to a single path. A subsequent call to `strokePath` or `fillPath` outlines or fills the shape defined by the path. It is not necessary to close a path in order to draw it.

## See Also

### Creating Paths (Lines, Curves, Arcs, and Shapes)

clip

Constrains the clipping region of the canvas to the current path.

isPointInPath

Determines whether a specified point is within the area defined by the current path.

