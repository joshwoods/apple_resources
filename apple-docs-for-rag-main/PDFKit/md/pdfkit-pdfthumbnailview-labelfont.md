

- PDFKit
- PDFThumbnailView
-  labelFont 

Instance Property

# labelFont

Returns the font used to label the thumbnails.

macOS 10.5+

``` source
@NSCopying @MainActor
var labelFont: NSFont? { get set }
```

## Return Value

The font used in the thumbnail labels.

## Discussion

Typically, the label of a thumbnail is the page number of the page it represents.

## See Also

### Working with Thumbnail View Display Characteristics

var maximumNumberOfColumns: Int

Returns the maximum number of columns of thumbnails the thumbnail view can display.

var backgroundColor: UIColor?

Returns the color used in the background of the thumbnail view.

