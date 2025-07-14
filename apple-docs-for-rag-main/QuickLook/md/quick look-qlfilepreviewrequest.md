

- Quick Look
-  QLFilePreviewRequest 

Class

# QLFilePreviewRequest

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
class QLFilePreviewRequest
```

## Topics

### Instance Properties

var fileURL: URL

The url of the file for which a preview is being requested.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### QuickLookUI symbols

class QLPreviewProvider

class QLPreviewReply

class QLPreviewReplyAttachment

protocol QLPreviewItem

protocol QLPreviewingController

For view based previews, the view controller that implements the QLPreviewingController protocol must at least implement one of the two following methods: -\[QLPreviewingController preparePreviewOfSearchableItemWithIdentifier:queryString:completionHandler:\], to generate previews for Spotlight searchable items. -\[QLPreviewingController preparePreviewOfFileAtURL:completionHandler:\], to generate previews for file URLs.

