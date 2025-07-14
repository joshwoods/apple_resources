

- Quick Look
-  QLPreviewReplyAttachment 

Class

# QLPreviewReplyAttachment

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
class QLPreviewReplyAttachment
```

## Topics

### Initializers

init(data: Data, contentType: UTType)

### Instance Properties

var contentType: UTType

The content type of the attachment for an html preview

var data: Data

The data content of an html preview

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

class QLFilePreviewRequest

class QLPreviewProvider

class QLPreviewReply

protocol QLPreviewItem

protocol QLPreviewingController

For view based previews, the view controller that implements the QLPreviewingController protocol must at least implement one of the two following methods: -\[QLPreviewingController preparePreviewOfSearchableItemWithIdentifier:queryString:completionHandler:\], to generate previews for Spotlight searchable items. -\[QLPreviewingController preparePreviewOfFileAtURL:completionHandler:\], to generate previews for file URLs.

