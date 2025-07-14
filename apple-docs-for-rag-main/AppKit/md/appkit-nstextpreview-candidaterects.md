

- AppKit
- NSTextPreview
-  candidateRects 

Instance Property

# candidateRects

Rectangles that define the specific portions of text to highlight.

macOS 15.2+

``` source
@MainActor
var candidateRects: [NSValue] { get }
```

## Discussion

At initialization time, you set this property to an array of NSValue objects, each of which contains an NSRect in the coordinate space of the target view. Each rectangle contains a bounding rectangle for text that is part of the preview. When applying visual effects, the system adds highlights only to the text in the specified rectangles.

## See Also

### Getting the preview details

var previewImage: CGImage

The image that contains the requested text from your view.

var presentationFrame: NSRect

The frame rectangle that places the preview image directly over the matching text.

