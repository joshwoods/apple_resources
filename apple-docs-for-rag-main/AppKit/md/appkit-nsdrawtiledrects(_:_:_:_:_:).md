

- AppKit
-  NSDrawTiledRects(\_:\_:\_:\_:\_:) 

Function

# NSDrawTiledRects(\_:\_:\_:\_:\_:)

Draws rectangles with borders.

macOS

``` source
func NSDrawTiledRects(
    _ boundsRect: NSRect,
    _ clipRect: NSRect,
    _ sides: UnsafePointer,
    _ grays: UnsafePointer,
    _ count: Int
) -> NSRect
```

## Parameters 

`boundsRect`  

The bounding rectangle (in the current coordinate system) in which to draw. Since this function is often used to draw the border of a view, this rectangle will typically be that view’s bounds rectangle. Only those parts of `boundsRect` that lie within the `clipRect` are actually drawn.

`clipRect`  

The clipping rectangle to use during drawing.

`sides`  

The sides of the rectangle for which you want to specify custom gray levels. Each side must have a corresponding entry in the `grays` parameter.

`grays`  

The gray levels to draw for each of the edges listed in the `sides` parameter.

`count`  

The number of 1.0-unit-wide slices to draw on the specified sides.

## Return Value

The rectangle that lies within the resulting border.

## Discussion

This is a generic function that can be used to draw different types of borders inside a given rectangle. These borders can be used to outline an area or to give rectangles the effect of being recessed from or elevated above the surface of the screen.

The `sides`, `grays`, and `count` parameters determine how thick the border is and what gray levels are used to form it. This function uses the `NSDivideRect` function to take successive 1.0-unit-wide slices from the sides of the rectangle specified by the `sides` parameter. Each slice is drawn using the corresponding gray level from the `grays` parameter. This function makes and draws these slices `count` number of times. If you specify the same side more than once, the second slice is drawn inside the first.

The following example uses this function to draw a bezeled border consisting of a 1.0–unit-wide white line at the top and on the left side and a 1.0-unit-wide dark-gray line inside a 1.0–unit-wide black line on the other two sides. The resulting rectangle inside this border is then filled in using light gray.

```
NSRectEdge mySides[] = {NSMinYEdge, NSMaxXEdge, NSMaxYEdge, NSMinXEdge,
                        NSMinYEdge, NSMaxXEdge};
float myGrays[] = {NSBlack, NSBlack, NSWhite, NSWhite,
                        NSDarkGray, NSDarkGray};
NSRect aRect, clipRect; // Assume exists

aRect = NSDrawTiledRects(aRect, clipRect, mySides, myGrays, 6);
[[NSColor grayColor] set];
NSRectFill(aRect);
```

In the preceding example, `mySides` is an array that specifies sides of a rectangle; for example, `NSMinYEdge` selects the side parallel to the x axis with the smallest y coordinate value. `myGrays` is an array that specifies the successive gray levels to be used in drawing parts of the border.

## See Also

### Drawing Rectangles

func NSEraseRect(NSRect)

Erases the specified rect by filling it with white.

func NSDrawGroove(NSRect, NSRect)

Draws a gray-filled rectangle with a groove border.

