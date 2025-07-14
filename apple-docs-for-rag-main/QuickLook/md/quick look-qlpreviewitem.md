

- Quick Look
-  QLPreviewItem 

Protocol

# QLPreviewItem

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
protocol QLPreviewItem : NSObjectProtocol
```

## Topics

### Instance Properties

var previewItemTitle: String?

var previewItemURL: URL?

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### QuickLookUI symbols

class QLFilePreviewRequest

class QLPreviewProvider

class QLPreviewReply

class QLPreviewReplyAttachment

protocol QLPreviewingController

For view based previews, the view controller that implements the QLPreviewingController protocol must at least implement one of the two following methods: -\[QLPreviewingController preparePreviewOfSearchableItemWithIdentifier:queryString:completionHandler:\], to generate previews for Spotlight searchable items. -\[QLPreviewingController preparePreviewOfFileAtURL:completionHandler:\], to generate previews for file URLs.

