

- PDFKit
- PDFThumbnailView
-  maximumNumberOfColumns 

Instance Property

# maximumNumberOfColumns

Returns the maximum number of columns of thumbnails the thumbnail view can display.

macOS 10.5+

``` source
@MainActor
var maximumNumberOfColumns: Int { get set }
```

## Return Value

The maximum number of columns of thumbnails the thumbnail view can display. If `0`, the thumbnail displays as many columns of thumbnails as fit in its size.

## See Also

### Working with Thumbnail View Display Characteristics

var labelFont: NSFont?

Returns the font used to label the thumbnails.

var backgroundColor: UIColor?

Returns the color used in the background of the thumbnail view.

