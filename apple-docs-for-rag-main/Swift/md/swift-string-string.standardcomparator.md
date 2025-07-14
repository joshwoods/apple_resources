

- Swift
- String
-  String.StandardComparator 

Structure

# String.StandardComparator

Compares `String`s using one of a fixed set of standard comparison algorithms.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct StandardComparator
```

## Topics

### Initializers

init(String.StandardComparator, order: SortOrder)

Create a `StandardComparator` from the given `StandardComparator` with the given new `order`.

### Type Properties

static let lexical: String.StandardComparator

Compares `String`s lexically.

static let localized: String.StandardComparator

Compares `String`s using a localized comparison in the current locale.

static let localizedStandard: String.StandardComparator

Compares `String`s as compared by the Finder.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable
- SortComparator

