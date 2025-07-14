

- Core Graphics
- CGDisplayStreamUpdateRectType
-  CGDisplayStreamUpdateRectType.movedRects 

Case

# CGDisplayStreamUpdateRectType.movedRects

The rectangles for the portions of the display that were simply moved from one part of the display to another.

Mac CatalystmacOS

``` source
case movedRects
```

## See Also

### Constants

case refreshedRects

The rectangles for the portions of the display that were redrawn.

case dirtyRects

The union of both rectangles that were redrawn and rectangles that were moved.

case reducedDirtyRects

The union is calculated and then simplified. This reduces the number of rectangles returned to your app, but it may report some pixels that were not actually changed.

