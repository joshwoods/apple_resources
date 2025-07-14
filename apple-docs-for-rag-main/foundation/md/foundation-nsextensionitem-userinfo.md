

- Foundation
- NSExtensionItem
-  userInfo 

Instance Property

# userInfo

An optional dictionary of keys and values corresponding to the extension item’s properties.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var userInfo: [AnyHashable : Any]? { get set }
```

## Discussion

If applicable to a particular extension type, additional information may be available in the `userInfo` dictionary. For example, in the context of an Action extension, the `userInfo` dictionary may contain values for the keys NSExtensionItemAttachmentsKey, NSExtensionItemAttributedContentTextKey, and NSExtensionItemAttributedTitleKey.

Important

Setting the userInfo dictionary after setting attachments, attributedContentText, or attributedTitle overrides those properties.

## See Also

### Identifying the Item

var attributedTitle: NSAttributedString?

An optional title for the item.

