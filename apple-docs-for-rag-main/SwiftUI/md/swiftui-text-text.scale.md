

- SwiftUI
- Text
-  Text.Scale 

Structure

# Text.Scale

Defines text scales

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Scale
```

## Overview

Text scale provides a way to pick a logical text scale relative to the base font which is used.

## Topics

### Getting built-in text scales

static let `default`: Text.Scale

Defines default text scale

static let secondary: Text.Scale

Defines secondary text scale

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Fitting text into available space

func textScale(Text.Scale, isEnabled: Bool) -> Text

Applies a text scale to the text.

enum TruncationMode

The type of truncation to apply to a line of text when it’s too long to fit in the available space.

