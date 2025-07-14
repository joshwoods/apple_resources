

- WeatherKit
-  HistoricalComparisons 

Structure

# HistoricalComparisons

A structure that represents the weather condition comparisons for a specific location. It’s a list of comparisons between current readings and historical averages. The list is ordered by significance of deviation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct HistoricalComparisons
```

## Topics

### Operators

static func == (HistoricalComparisons, HistoricalComparisons) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var comparisons: [HistoricalComparison]

A list of comparisons between current readings and historical averages, ordered by significance of deviation.

var endIndex: HistoricalComparisons.Index

The end index for the historical comparisons.

var metadata: WeatherMetadata

Descriptive information about the weather comparisons data.

var startIndex: HistoricalComparisons.Index

The start index for the historical comparisons.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Subscripts

subscript(HistoricalComparisons.Index) -> HistoricalComparisons.Element

The historical comparison at the provided index.

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
- Sequence

