

- WeatherKit
-  DailyWeatherSummary 

Structure

# DailyWeatherSummary

A structure that holds a collection of day weather summaries.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct DailyWeatherSummary where T : Decodable, T : Encodable, T : Equatable, T : Sendable
```

## Topics

### Operators

static func == (DailyWeatherSummary&lt;T>, DailyWeatherSummary&lt;T>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var days: [T]

An ordered collection of day weather summaries of type `T`, for each requested day.

var endIndex: DailyWeatherSummary&lt;T>.Index

The end index for the daily weather summaries.

var metadata: WeatherMetadata

Descriptive information about the weather statistics data.

var startIndex: DailyWeatherSummary&lt;T>.Index

The start index for the daily weather summaries.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Subscripts

subscript(DailyWeatherSummary&lt;T>.Index) -> DailyWeatherSummary&lt;T>.Element

The day weather summary at the provided index.

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

Equatable Implementations

RandomAccessCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Decodable
- Encodable
- Equatable
- RandomAccessCollection
- Sendable
- Sequence

