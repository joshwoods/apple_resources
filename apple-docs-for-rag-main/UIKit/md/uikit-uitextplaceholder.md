

- UIKit
-  UITextPlaceholder 

Class

# UITextPlaceholder

A placeholder object that reserves visual space in a text input view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UITextPlaceholder
```

## Topics

### Accessing the selection rectangles

var rects: [UITextSelectionRect]

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
- Sendable

## See Also

### Managing placeholders

func insertTextPlaceholder(with: CGSize) -> UITextPlaceholder

Inserts a placeholder object to reserve visual space during text input.

func remove(UITextPlaceholder)

Removes a placeholder object from the text input view.

