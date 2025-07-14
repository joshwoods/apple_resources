

- UIKit
-  UILetterformAwareSizingRule 

Enumeration

# UILetterformAwareSizingRule

Constants that specify typographic bounds-sizing behavior to handle text in fonts with oversize characters.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
enum UILetterformAwareSizingRule
```

## Overview

For more information on typographic bounds sizing behavior, see UILetterformAwareAdjusting.

## Topics

### Setting bounds-sizing behavior

case oversize

Bounds-sizing behavior that displays oversize characters fully but may negatively impact typographic alignment.

case typographic

Standard typographic bounds-sizing behavior, which may clip oversize characters.

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

### Specifying text-sizing behavior

var sizingRule: UILetterformAwareSizingRule

The typographic bounds-sizing behavior that handles text with fonts that contain oversize characters.

**Required**

