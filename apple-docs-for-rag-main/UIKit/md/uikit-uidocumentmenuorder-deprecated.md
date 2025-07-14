

- UIKit
-  UIDocumentMenuOrder Deprecated

Enumeration

# UIDocumentMenuOrder

The insertion point for custom menu items.

iOS 8.0–11.0DeprecatediPadOS 8.0–11.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
enum UIDocumentMenuOrder
```

## Topics

### Constants

case first

The top item in the document menu.

case last

The bottom item in the document menu.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring a document menu

func addOption(withTitle: String, image: UIImage?, order: UIDocumentMenuOrder, handler: () -> Void)

Adds a custom menu item to the list of document pickers.

Deprecated

