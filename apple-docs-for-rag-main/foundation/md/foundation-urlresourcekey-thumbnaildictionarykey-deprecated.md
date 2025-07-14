

- Foundation
- URLResourceKey
-  thumbnailDictionaryKey Deprecated

Type Property

# thumbnailDictionaryKey

A dictionary of NSImage/UIImage objects keyed by size (read-write). See URLThumbnailDictionaryItem for a list of possible keys.

iOS 8.0–15.0DeprecatediPadOS 8.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.10–12.0DeprecatedtvOS 9.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–8.0Deprecated

``` source
static let thumbnailDictionaryKey: URLResourceKey
```

Deprecated

Use the QuickLookThumbnailing framework and extension point instead

## See Also

### Thumbnail keys

static let thumbnailKey: URLResourceKey

All thumbnails as a single NSImage (read-write).

Deprecated

struct URLThumbnailDictionaryItem

Possible keys for the thumbnailDictionaryKey dictionary.

