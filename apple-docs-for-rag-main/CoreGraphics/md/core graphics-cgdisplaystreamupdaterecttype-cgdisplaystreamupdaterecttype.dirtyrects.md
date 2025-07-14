

- Core Graphics
- CGDisplayStreamUpdateRectType
-  CGDisplayStreamUpdateRectType.dirtyRects 

Case

# CGDisplayStreamUpdateRectType.dirtyRects

The union of both rectangles that were redrawn and rectangles that were moved.

Mac CatalystmacOS

``` source
case dirtyRects
```

## See Also

### Constants

case refreshedRects

The rectangles for the portions of the display that were redrawn.

case movedRects

The rectangles for the portions of the display that were simply moved from one part of the display to another.

case reducedDirtyRects

The union is calculated and then simplified. This reduces the number of rectangles returned to your app, but it may report some pixels that were not actually changed.

