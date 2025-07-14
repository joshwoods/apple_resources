

- Foundation
- NSExtensionItem
-  attributedTitle 

Instance Property

# attributedTitle

An optional title for the item.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var attributedTitle: NSAttributedString? { get set }
```

## Discussion

Important

Alternatively, you can set attributed content in the userInfo dictionary using the NSExtensionItemAttributedTitleKey key. However, setting the userInfo dictionary after setting attributedTitle overrides this property.

## See Also

### Related Documentation

App Extension Programming Guide

### Identifying the Item

var userInfo: [AnyHashable : Any]?

An optional dictionary of keys and values corresponding to the extension item’s properties.

