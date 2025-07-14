

- AppKit
- NSClipView
-  drawsBackground 

Instance Property

# drawsBackground

A Boolean value that indicates if the clip view draws its background color.

macOS

``` source
@MainActor
var drawsBackground: Bool { get set }
```

## Discussion

If your NSClipView is enclosed in an NSScrollView, you should set the drawsBackground property on the NSScrollView. Setting this property to false on an NSScrollView has the added effect of setting the NSClipView property copiesOnScroll to false. The side effect of setting the drawsBackground property on the NSClipView is the appearance of “trails” (vestiges of previous drawing) in the document view as it is scrolled.

## See Also

### Working with Background Color

var backgroundColor: NSColor

The color of the clip view’s background.

