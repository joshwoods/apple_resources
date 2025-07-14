

- Quick Look UI
-  QLPreviewReplyAttachment 

Class

# QLPreviewReplyAttachment

An attachment for a Quick Look preview reply that provides additional content for the system to display a preview.

macOS 12.0+

``` source
class QLPreviewReplyAttachment
```

## Overview

When providing a data-based Quick Look preview with HTML, use QLPreviewReplyAttachment to include images, CSS, and other linked content in the HTML of the preview.

Reference content in your html using the `CID` notation for the reference. For instance, if your HTML preview response includes an image, create a QLPreviewReplyAttachment with the image, add it the reply’s attachments with an associated string, and reference the image with the associated string, prefixed by `cid:`. The following example illustrates returning HTML as a preview reply with an image as an attachment:

```
let reply = QLPreviewReply(dataOfContentType: .html,
                           contentSize: CGSize(width: 750, height: 500)) { htmlReply in
    let content = """

                  Preview

                  """
    guard let contentData = content.data(using: .utf8) else {
        throw PreviewError.previewSetupFailure("Unable to encode preview content")
    }
    guard let imageFileURL = Bundle.main.url(forResource: "yourImage",
                                             withExtension: "jpg") else {
        throw PreviewError.previewSetupFailure("unable to load image")
    }
    let imageData = try Data(contentsOf: imageFileURL)

    htmlReply.attachments["exampleImage"] = QLPreviewReplyAttachment(data: imageData,
                                                                     contentType: .jpeg)
    return contentData
}
reply.title = "HTML Preview Example"

```

## Topics

### Creating a preview reply attachment

init(data: Data, contentType: UTType)

Creates a preview reply attachment with the specified type.

### Inspecting a preview reply attachment

var contentType: UTType

The content type of the preview attachment.

var data: Data

The data of the preview attachment.

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

class QLPreviewReply

The class you create when providing a data-based Quick Look preview extension.

