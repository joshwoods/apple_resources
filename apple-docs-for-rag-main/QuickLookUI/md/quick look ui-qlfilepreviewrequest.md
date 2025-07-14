

- Quick Look UI
-  QLFilePreviewRequest 

Class

# QLFilePreviewRequest

A Quick Look preview request that indicates the content to preview.

macOS 12.0+

``` source
class QLFilePreviewRequest
```

## Overview

The system provides a QLFilePreviewRequest to the providePreview(for:completionHandler:) method of your data-based Quick Look extension.

## Topics

### Inspecting the preview request

var fileURL: URL

The URL that indicates the content to preview.

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

### Data-based Preview Extensions

class QLPreviewProvider

A class that you subclass to provide a data-based Quick Look preview extension.

class QLPreviewReply

The class you create when providing a data-based Quick Look preview extension.

class QLPreviewReplyAttachment

An attachment for a Quick Look preview reply that provides additional content for the system to display a preview.

