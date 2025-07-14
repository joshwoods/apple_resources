

- UIKit
-  UIContextMenuInteractionCommitStyle 

Enumeration

# UIContextMenuInteractionCommitStyle

Constants that control the interaction commit style.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum UIContextMenuInteractionCommitStyle
```

## Topics

### Interaction Styles

case dismiss

An interaction with no animations.

case pop

An interaction that uses animations.

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

### Specifying the Commit Style

var preferredCommitStyle: UIContextMenuInteractionCommitStyle

The preferred animation style triggered when the user taps the preview.

**Required**

