

- WeatherKit
-  WeatherChanges 

Structure

# WeatherChanges

A structure that represents the Weather Change forecast. It provides a qualitative assessment of whether upcoming weather is significantly different from prior conditions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct WeatherChanges
```

## Topics

### Instance Properties

var changes: [WeatherChange]

A list of forecasted weather changes, in chronological order.

var endIndex: WeatherChanges.Index

The end index for the weather changes.

var metadata: WeatherMetadata

Descriptive information about the weather change data.

var startIndex: WeatherChanges.Index

The start index for the weather changes.

### Subscripts

subscript(WeatherChanges.Index) -> WeatherChanges.Element

The weather change at the provided index.

### Type Aliases

typealias Element

A type representing the sequence’s elements.

typealias Index

A type that represents a position in the collection.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

RandomAccessCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- Decodable
- Encodable
- Equatable
- RandomAccessCollection
- Sequence

