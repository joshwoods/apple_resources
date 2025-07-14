

- Quick Look UI
-  QLPreviewProvider 

Class

# QLPreviewProvider

A class that you subclass to provide a data-based Quick Look preview extension.

macOS 12.0+

``` source
class QLPreviewProvider
```

## Overview

When you subclass QLPreviewProvider, conform your subclass QLPreviewingController.

To provide a data-based Quick Look extension, make the following modifications to your Info.plist file:

- Set the Boolean key `QLIsDataBasedPreview` to `true`.

- Add the type identifiers for your extension’s supported content types to the `QLSupportedContentTypes` array.

- Change the value of `NSExtensionPrincipalClass` to the name of your subclass. For example, if you named your subclass `PreviewProvider`, set the value to `$(PRODUCT_MODULE_NAME).PreviewProvider`.

After updating the extension’s `Info.plist` file, implement the providePreview(for:completionHandler:) method to return a QLPreviewReply for the provided QLFilePreviewRequest.

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

### Data-based Preview Extensions

class QLFilePreviewRequest

A Quick Look preview request that indicates the content to preview.

class QLPreviewReply

The class you create when providing a data-based Quick Look preview extension.

class QLPreviewReplyAttachment

An attachment for a Quick Look preview reply that provides additional content for the system to display a preview.

