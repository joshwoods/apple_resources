

- Foundation
- PersonNameComponents
- PersonNameComponents.FormatStyle
-  PersonNameComponents.FormatStyle.Style 

Enumeration

# PersonNameComponents.FormatStyle.Style

The type that represents the style of the formatted result.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Style
```

## Overview

The style type describes a length of the string representation of the name. The available values are PersonNameComponents.FormatStyle.Style.long, PersonNameComponents.FormatStyle.Style.medium, PersonNameComponents.FormatStyle.Style.short, and PersonNameComponents.FormatStyle.Style.abbreviated.

## Topics

### Enumeration Cases

case abbreviated

Specifies an abbreviated person name components style.

case long

Specifies a long person name components style.

case medium

Specifies a medium person name components style.

case short

Specifies a short person name components style.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Modifying a Format Style

var style: PersonNameComponents.FormatStyle.Style

Specifies the style of the formatted result.

var locale: Locale

The locale to use when formatting the person name components.

var attributed: PersonNameComponents.AttributedStyle

The style used to create a locale-aware attributed string representation of an instance of person name components.

