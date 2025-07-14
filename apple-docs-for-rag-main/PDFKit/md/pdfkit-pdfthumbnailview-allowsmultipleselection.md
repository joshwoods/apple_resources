

- PDFKit
- PDFThumbnailView
-  allowsMultipleSelection 

Instance Property

# allowsMultipleSelection

Returns a Boolean value indicating whether users can select multiple thumbnails in the thumbnail view at one time.

macOS 10.5+

``` source
@MainActor
var allowsMultipleSelection: Bool { get set }
```

## Return Value

true if users can select multiple thumbnails simultaneously, false otherwise.

## Discussion

By default, `PDFThumbnailView` allows only a single thumbnail to be selected at one time. When this is the case, you can get the PDF page that corresponds to the selected thumbnail using the `PDFView` method currentPage.

When multiple selections are enabled, however, you must use selectedPages to get the pages that correspond to the set of selected thumbnails.

## See Also

### Managing the Behavior of a Thumbnail View

var allowsDragging: Bool

Returns a Boolean value indicating whether users can drag thumbnails (that is, re-order pages in the document) within the thumbnail view.

var selectedPages: [PDFPage]?

Returns an array of PDF pages that correspond to the selected thumbnails in the thumbnail view.

