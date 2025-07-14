

- AppKit
- NSTextPreview
-  presentationFrame 

Instance Property

# presentationFrame

The frame rectangle that places the preview image directly over the matching text.

macOS 15.2+

``` source
@MainActor
var presentationFrame: NSRect { get }
```

## Discussion

You specify this value at initialization time. The system uses it to position the preview image over the text in your view. Make sure the frame rectangle is in your view’s coordinate space.

## See Also

### Getting the preview details

var previewImage: CGImage

The image that contains the requested text from your view.

var candidateRects: [NSValue]

Rectangles that define the specific portions of text to highlight.

