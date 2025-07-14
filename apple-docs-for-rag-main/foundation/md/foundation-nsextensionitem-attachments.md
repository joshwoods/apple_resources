

- Foundation
- NSExtensionItem
-  attachments 

Instance Property

# attachments

An optional array of media data associated with the extension item.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var attachments: [NSItemProvider]? { get set }
```

## Discussion

Populate this array with images, videos, URLs, and so on. It’s not meant to be an array of alternative data formats or types, but is instead a collection to include in a social media post, for example. These items are always typed NSItemProvider.

Important

Alternatively, you can set attachments in the userInfo dictionary using the NSExtensionItemAttachmentsKey key. However, setting the userInfo dictionary after setting attachments will override this property.

## See Also

### Item Contents

var attributedContentText: NSAttributedString?

An optional string describing the extension item content.

