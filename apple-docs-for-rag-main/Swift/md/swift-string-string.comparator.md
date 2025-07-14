

- Swift
- String
-  String.Comparator 

Structure

# String.Comparator

A `String` comparison performed using the given comparison options and locale.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Comparator
```

## Topics

### Initializers

init(String.StandardComparator)

Creates a `String.Comparator` that represents the same comparison as the given `String.StandardComparator`.

init(options: String.CompareOptions, locale: Locale?, order: SortOrder)

Creates a `String.Comparator` with the given `CompareOptions` and `Locale`.

### Instance Properties

let locale: Locale?

The locale to use for comparison if the comparator is localized, otherwise nil.

let options: String.CompareOptions

The options to use for comparison.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable
- SortComparator

