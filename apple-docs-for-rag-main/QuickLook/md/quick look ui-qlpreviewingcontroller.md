

- Quick Look UI
-  QLPreviewingController 

Protocol

# QLPreviewingController

A protocol for implementing a custom controller to create previews of files.

macOS 12.0+

``` source
protocol QLPreviewingController : NSObjectProtocol
```

## Overview

A controller that implements the `QLPreviewingController` protocol must at least implement preparePreviewOfSearchableItem(identifier:queryString:completionHandler:) or preparePreviewOfFile(at:completionHandler:).

## Topics

### Instance Methods

func preparePreviewOfFile(at: URL, completionHandler: ((any Error)?) -> Void)

Prepares the preview of a file at the specified file’s URL.

func preparePreviewOfSearchableItem(identifier: String, queryString: String?, completionHandler: ((any Error)?) -> Void)

Prepares the preview for a file by using the data from Spotlight’s searchable item.

func providePreview(for: QLFilePreviewRequest, completionHandler: (QLPreviewReply?, (any Error)?) -> Void)

Prepares the preview of a file identified within a file preview request.

## Relationships

### Inherits From

- NSObjectProtocol

