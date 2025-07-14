

- Quick Look
-  QLPreviewingController 

Protocol

# QLPreviewingController

For view based previews, the view controller that implements the QLPreviewingController protocol must at least implement one of the two following methods: -\[QLPreviewingController preparePreviewOfSearchableItemWithIdentifier:queryString:completionHandler:\], to generate previews for Spotlight searchable items. -\[QLPreviewingController preparePreviewOfFileAtURL:completionHandler:\], to generate previews for file URLs.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
protocol QLPreviewingController : NSObjectProtocol
```

## Overview

The main preview should be presented by the view controller implementing QLPreviewingController. Avoid presenting additional view controllers over your QLPreviewingController. For Catalyst compatibility, avoid using gesture recognizers that take interactions over large portions of the view to avoid collisions with standard macOS preview behaviors. Avoid holding the file open during the duration of the preview. If access to the file is necessary for interaction, it is best to keep the file open only for the duration of the interaction.

For data-based previews, subclass QLPreviewProvider which conforms to this protocol.

## Topics

### Instance Methods

func preparePreviewOfFile(at: URL, completionHandler: ((any Error)?) -> Void)

func preparePreviewOfSearchableItem(identifier: String, queryString: String?, completionHandler: ((any Error)?) -> Void)

func providePreview(for: QLFilePreviewRequest, completionHandler: (QLPreviewReply?, (any Error)?) -> Void)

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### QuickLookUI symbols

class QLFilePreviewRequest

class QLPreviewProvider

class QLPreviewReply

class QLPreviewReplyAttachment

protocol QLPreviewItem

