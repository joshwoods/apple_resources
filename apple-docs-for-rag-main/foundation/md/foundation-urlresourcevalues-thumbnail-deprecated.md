

- Foundation
- URLResourceValues
-  thumbnail Deprecated

Instance Property

# thumbnail

A thumbnail image of the URL.

macOS 10.10–12.0Deprecated

``` source
var thumbnail: NSImage? { get }
```

Deprecated

Use the QuickLookThumbnailing framework and extension point instead

## Discussion

The URL populates ths property by retrieving the thumbnailKey from the resource values, and is `nil` if there’s no value for the key.

## See Also

### Thumbnail values

var thumbnailDictionary: [URLThumbnailDictionaryItem : UIImage]?

A dictionary of UIKit image objects keyed by size.

Deprecated

var thumbnailDictionary: [URLThumbnailDictionaryItem : NSImage]?

A dictionary of AppKit image objects keyed by size.

Deprecated

