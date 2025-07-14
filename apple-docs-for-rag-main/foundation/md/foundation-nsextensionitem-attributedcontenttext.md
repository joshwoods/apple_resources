

- Foundation
- NSExtensionItem
-  attributedContentText 

Instance Property

# attributedContentText

An optional string describing the extension item content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var attributedContentText: NSAttributedString? { get set }
```

## Discussion

Important

Alternatively, you can set attributed content in the userInfo dictionary using the NSExtensionItemAttributedContentTextKey key. However, setting the userInfo dictionary after setting attributedContentText overrides this property.

## See Also

### Item Contents

var attachments: [NSItemProvider]?

An optional array of media data associated with the extension item.

