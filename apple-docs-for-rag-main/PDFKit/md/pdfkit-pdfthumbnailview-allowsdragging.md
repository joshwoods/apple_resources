

- PDFKit
- PDFThumbnailView
-  allowsDragging 

Instance Property

# allowsDragging

Returns a Boolean value indicating whether users can drag thumbnails (that is, re-order pages in the document) within the thumbnail view.

macOS 10.5+

``` source
@MainActor
var allowsDragging: Bool { get set }
```

## Return Value

true if users can re-order pages by dragging thumbnails, false otherwise.

## See Also

### Managing the Behavior of a Thumbnail View

var allowsMultipleSelection: Bool

Returns a Boolean value indicating whether users can select multiple thumbnails in the thumbnail view at one time.

var selectedPages: [PDFPage]?

Returns an array of PDF pages that correspond to the selected thumbnails in the thumbnail view.

