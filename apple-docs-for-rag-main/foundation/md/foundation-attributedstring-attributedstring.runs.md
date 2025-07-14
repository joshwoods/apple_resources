

- Foundation
- AttributedString
-  AttributedString.Runs 

Structure

# AttributedString.Runs

An iterable view into segments of the attributed string, each of which indicates where a run of identical attributes begins or ends.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Runs
```

## Topics

### Structures

struct AttributesSlice1

struct AttributesSlice2

struct AttributesSlice3

struct AttributesSlice4

struct AttributesSlice5

struct Run

### Subscripts

subscript&lt;T>(T.Type) -> AttributedString.Runs.AttributesSlice1&lt;T>

subscript&lt;T>(KeyPath&lt;AttributeDynamicLookup, T>) -> AttributedString.Runs.AttributesSlice1&lt;T>

subscript(AttributedString.Index) -> AttributedString.Runs.Run

subscript&lt;T, U>(T.Type, U.Type) -> AttributedString.Runs.AttributesSlice2&lt;T, U>

subscript&lt;T, U>(KeyPath&lt;AttributeDynamicLookup, T>, KeyPath&lt;AttributeDynamicLookup, U>) -> AttributedString.Runs.AttributesSlice2&lt;T, U>

subscript&lt;T, U, V>(KeyPath&lt;AttributeDynamicLookup, T>, KeyPath&lt;AttributeDynamicLookup, U>, KeyPath&lt;AttributeDynamicLookup, V>) -> AttributedString.Runs.AttributesSlice3&lt;T, U, V>

subscript&lt;T, U, V>(T.Type, U.Type, V.Type) -> AttributedString.Runs.AttributesSlice3&lt;T, U, V>

subscript&lt;T, U, V, W>(T.Type, U.Type, V.Type, W.Type) -> AttributedString.Runs.AttributesSlice4&lt;T, U, V, W>

subscript&lt;T, U, V, W>(KeyPath&lt;AttributeDynamicLookup, T>, KeyPath&lt;AttributeDynamicLookup, U>, KeyPath&lt;AttributeDynamicLookup, V>, KeyPath&lt;AttributeDynamicLookup, W>) -> AttributedString.Runs.AttributesSlice4&lt;T, U, V, W>

subscript&lt;T, U, V, W, X>(KeyPath&lt;AttributeDynamicLookup, T>, KeyPath&lt;AttributeDynamicLookup, U>, KeyPath&lt;AttributeDynamicLookup, V>, KeyPath&lt;AttributeDynamicLookup, W>, KeyPath&lt;AttributeDynamicLookup, X>) -> AttributedString.Runs.AttributesSlice5&lt;T, U, V, W, X>

subscript&lt;T, U, V, W, X>(T.Type, U.Type, V.Type, W.Type, X.Type) -> AttributedString.Runs.AttributesSlice5&lt;T, U, V, W, X>

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- CustomStringConvertible
- Equatable
- Sendable
- Sequence

## See Also

### Accessing Views into the Attributed String

struct CharacterView

A view into the underlying storage of the attributed string, as Unicode characters.

struct UnicodeScalarView

A view into the underlying storage of the attributed string, as Unicode scalars.

