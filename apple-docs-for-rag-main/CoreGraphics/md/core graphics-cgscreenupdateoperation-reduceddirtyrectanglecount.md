

- Core Graphics
- CGScreenUpdateOperation
-  reducedDirtyRectangleCount 

Type Property

# reducedDirtyRectangleCount

Mac CatalystmacOS

``` source
static var reducedDirtyRectangleCount: CGScreenUpdateOperation { get }
```

## Discussion

When presented as part of the requested operations to the function CGWaitForScreenUpdateRects(_:_:_:_:_:), specifies that the function should try to minimize the number of rectangles returned to represent the changed areas of the display. The function may combine adjacent rectangles within a larger bounding rectangle, which may include unmodified areas of the display.

## See Also

### Constants

static var refresh: CGScreenUpdateOperation

A screen-refresh operation.

static var move: CGScreenUpdateOperation

A screen-move operation.

