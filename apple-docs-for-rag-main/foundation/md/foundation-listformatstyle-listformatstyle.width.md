

- Foundation
- ListFormatStyle
-  ListFormatStyle.Width 

Enumeration

# ListFormatStyle.Width

The type representing the width of a list.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Width
```

## Overview

The possible values of a width are `standard`, `short`, and `narrow`.

## Topics

### Widths

case standard

Specifies a standard list style.

case short

Specifies a short list style.

case narrow

Specifies a narrow list style, the shortest list style.

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

### Modifying a list format style

var width: ListFormatStyle&lt;Style, Base>.Width

The size of the list.

var listType: ListFormatStyle&lt;Style, Base>.ListType

The type of the list.

enum ListType

A type that describes whether the returned list contains cumulative or alternative elements.

var locale: Locale

The locale to use when formatting items in the list.

