

- Foundation
- ListFormatStyle
-  ListFormatStyle.ListType 

Enumeration

# ListFormatStyle.ListType

A type that describes whether the returned list contains cumulative or alternative elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum ListType
```

## Overview

The possible values of a listType are `and` and `or`.

## Topics

### List types

case and

Specifies an *and* list type.

case or

Specifies an *or* list type.

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

enum Width

The type representing the width of a list.

var listType: ListFormatStyle&lt;Style, Base>.ListType

The type of the list.

var locale: Locale

The locale to use when formatting items in the list.

