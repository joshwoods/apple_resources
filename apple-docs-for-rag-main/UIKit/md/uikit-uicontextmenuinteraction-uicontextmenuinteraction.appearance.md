

- UIKit
- UIContextMenuInteraction
-  UIContextMenuInteraction.appearance 

Enumeration

# UIContextMenuInteraction.appearance

Constants that describe the appearance of the menu.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
enum appearance
```

## Topics

### Constants

case unknown

No menu appearance.

case rich

A modal menu with an optional preview.

case compact

A nonmodal, compact menu with no preview.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the menu appearance

var menuAppearance: UIContextMenuInteraction.appearance

The appearance of the context menu.

