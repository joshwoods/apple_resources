

- AppKit
- NSImage
-  backgroundColor 

Instance Property

# backgroundColor

The background color for the image.

macOS

``` source
@NSCopying
var backgroundColor: NSColor { get set }
```

## Discussion

The background color is visible only if the drawn image representation does not completely cover all of the pixels available for the image’s current size. The background color is ignored for cached image representations; such caches are always created with a white background. Assigning a new background color does not cause the receiver to recache itself.

The default color is transparent, as returned by the clear method of `NSColor`.

## See Also

### Related Documentation

func recache()

Invalidates and frees offscreen caches of all image representations.

### Managing Drawing Options

var isValid: Bool

A Boolean value that indicates whether it is possible to draw an image representation.

var capInsets: NSEdgeInsets

The cap insets for the image.

var resizingMode: NSImage.ResizingMode

The resizing mode for the image.

enum ResizingMode

Constants that describe the resizing mode for the image.

