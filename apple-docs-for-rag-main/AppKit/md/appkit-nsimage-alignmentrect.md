

- AppKit
- NSImage
-  alignmentRect 

Instance Property

# alignmentRect

A rectangle that you can use to position the image during layout.

macOS 10.5+

``` source
var alignmentRect: NSRect { get set }
```

## Discussion

Alignment rectangles specify baselines that you can use to position the content of an image more accurately. These baselines are merely hints that your own code can use to determine positioning. The `NSImage` class does not use this rectangle during drawing; however, instances of NSCell typically use this information when laying out images within their boundaries.

For example, if you have a 20 x 20 pixel icon that includes a glow effect, you might set the alignment rectangle to `{{2, 2}, {16, 16}}` to indicate the position of the underlying icon without the glow effect. This property defaults to a rectangle with an origin of `{0, 0}` and a size that matches the size of the image.

