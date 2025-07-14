

- SwiftUI
- Text
-  Text.TruncationMode 

Enumeration

# Text.TruncationMode

The type of truncation to apply to a line of text when it’s too long to fit in the available space.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum TruncationMode
```

## Overview

When a text view contains more text than it’s able to display, the view might truncate the text and place an ellipsis (…) at the truncation point. Use the truncationMode(_:) modifier with one of the `TruncationMode` values to indicate which part of the text to truncate, either at the beginning, in the middle, or at the end.

## Topics

### Getting text truncation modes

case head

Truncate at the beginning of the line.

case middle

Truncate in the middle of the line.

case tail

Truncate at the end of the line.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Fitting text into available space

func textScale(Text.Scale, isEnabled: Bool) -> Text

Applies a text scale to the text.

struct Scale

Defines text scales

