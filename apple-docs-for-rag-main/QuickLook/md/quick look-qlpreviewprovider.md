

- Quick Look
-  QLPreviewProvider 

Class

# QLPreviewProvider

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
class QLPreviewProvider
```

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSExtensionRequestHandling
- NSObjectProtocol

## See Also

### QuickLookUI symbols

class QLFilePreviewRequest

class QLPreviewReply

class QLPreviewReplyAttachment

protocol QLPreviewItem

protocol QLPreviewingController

For view based previews, the view controller that implements the QLPreviewingController protocol must at least implement one of the two following methods: -\[QLPreviewingController preparePreviewOfSearchableItemWithIdentifier:queryString:completionHandler:\], to generate previews for Spotlight searchable items. -\[QLPreviewingController preparePreviewOfFileAtURL:completionHandler:\], to generate previews for file URLs.

