

- AppKit
- NSScrollView
-  backgroundColor 

Instance Property

# backgroundColor

The color of the content view’s background.

macOS

``` source
@NSCopying @MainActor
var backgroundColor: NSColor { get set }
```

## Discussion

This color is used to paint areas inside the content view that aren’t covered by the document view.

## See Also

### Related Documentation

var backgroundColor: NSColor

The color of the clip view’s background.

### Managing Graphics Attributes

var drawsBackground: Bool

A Boolean that indicates whether the scroll view draws its background.

var borderType: NSBorderType

A value that specifies the appearance of the scroll view’s border.

var documentCursor: NSCursor?

The content view’s document cursor.

