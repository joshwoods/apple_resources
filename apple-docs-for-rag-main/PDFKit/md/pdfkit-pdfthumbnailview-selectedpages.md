

- PDFKit
- PDFThumbnailView
-  selectedPages 

Instance Property

# selectedPages

Returns an array of PDF pages that correspond to the selected thumbnails in the thumbnail view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var selectedPages: [PDFPage]? { get }
```

## Return Value

An array of PDF pages that correspond to the thumbnails selected in the thumbnail view.

## Discussion

If the thumbnail view allows multiple selections (if allowsMultipleSelection returns true), you can use this method to get the PDF pages that correspond to the selected thumbnails.

## See Also

### Managing the Behavior of a Thumbnail View

var allowsDragging: Bool

Returns a Boolean value indicating whether users can drag thumbnails (that is, re-order pages in the document) within the thumbnail view.

var allowsMultipleSelection: Bool

Returns a Boolean value indicating whether users can select multiple thumbnails in the thumbnail view at one time.

