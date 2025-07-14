

- Quick Look UI
-  QLPreviewReply 

Class

# QLPreviewReply

The class you create when providing a data-based Quick Look preview extension.

macOS 12.0+

``` source
class QLPreviewReply
```

## Overview

Create an instance of QLPreviewReply from the method providePreview(for:completionHandler:) in your subclass of QLPreviewProvider. Create an instance to return data; for example, an image, PDF, or HTML; that the system displays as the preview for the content that the system indicates with QLFilePreviewRequest.

## Topics

### Creating a preview reply

init(fileURL: URL)

Creates a preview reply from an existing file URL.

### Create a PDF preview reply

convenience init(forPDFWithPageSize: CGSize, createDocumentUsing: (QLPreviewReply) throws -> PDFDocument)

### Generating a preview reply

convenience init(dataOfContentType: UTType, contentSize: CGSize, createDataUsing: (QLPreviewReply) throws -> Data)

### Drawing a preview reply

convenience init(contextSize: CGSize, isBitmap: Bool, drawUsing: (CGContext, QLPreviewReply) throws -> Void)

### Inspecting a preview reply

var title: String

The title for the system to display with the preview.

var attachments: [String : QLPreviewReplyAttachment]

The attachments for a preview reply that provide additional data for the system to display the preview.

var stringEncoding: String.Encoding

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

class QLFilePreviewRequest

A Quick Look preview request that indicates the content to preview.

class QLPreviewReplyAttachment

An attachment for a Quick Look preview reply that provides additional content for the system to display a preview.

