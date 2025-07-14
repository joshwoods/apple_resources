

- Foundation
-  URLThumbnailDictionaryItem 

Structure

# URLThumbnailDictionaryItem

Possible keys for the thumbnailDictionaryKey dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct URLThumbnailDictionaryItem
```

## Topics

### Creating a Thumbnail Dictionary Key

init(String)

Creates a thumbnail dictionary item key from the provided constant string.

init(rawValue: String)

### Constants

static let NSThumbnail1024x1024SizeKey: URLThumbnailDictionaryItem

A 1024 x 1024 pixel thumbnail as a `UIImage` on iOS or an `NSImage` in macOS.

Deprecated

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Thumbnail keys

static let thumbnailKey: URLResourceKey

All thumbnails as a single NSImage (read-write).

Deprecated

static let thumbnailDictionaryKey: URLResourceKey

A dictionary of NSImage/UIImage objects keyed by size (read-write). See URLThumbnailDictionaryItem for a list of possible keys.

Deprecated

