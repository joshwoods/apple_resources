

- AppKit
- NSTextPreview
-  previewImage 

Instance Property

# previewImage

The image that contains the requested text from your view.

macOS 15.2+

``` source
@MainActor
var previewImage: CGImage { get }
```

## Discussion

You specify this image at initialization time. The system uses it to implement any visual effects involving your view’s text. Create the image with your text on a transparent background.

## See Also

### Getting the preview details

var presentationFrame: NSRect

The frame rectangle that places the preview image directly over the matching text.

var candidateRects: [NSValue]

Rectangles that define the specific portions of text to highlight.

