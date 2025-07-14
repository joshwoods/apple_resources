

- AppKit
- NSScrollView
-  drawsBackground 

Instance Property

# drawsBackground

A Boolean that indicates whether the scroll view draws its background.

macOS

``` source
@MainActor
var drawsBackground: Bool { get set }
```

## Discussion

When the value of this property is true, the scroll view cell fills the background with its background color.

If the scroll view encloses an `NSClipView`, setting this property to false also sets the `NSClipView` property copiesOnScroll to false. The side effect of setting `drawsBackground` directly on the `NSClipView` instead is the appearance of “trails” (vestiges of previous drawing) in the document view as it is scrolled.

## See Also

### Related Documentation

var drawsBackground: Bool

A Boolean value that indicates if the clip view draws its background color.

var copiesOnScroll: Bool

A Boolean value that indicates if the clip view copies rendered images while scrolling.

Deprecated

### Managing Graphics Attributes

var backgroundColor: NSColor

The color of the content view’s background.

var borderType: NSBorderType

A value that specifies the appearance of the scroll view’s border.

var documentCursor: NSCursor?

The content view’s document cursor.

