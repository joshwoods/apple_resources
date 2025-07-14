

- Swift
-  Decodable 

Protocol

# Decodable

A type that can decode itself from an external representation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol Decodable
```

## Topics

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

**Required** Default implementation provided.

## Relationships

### Inherited By

- SIMD

### Conforming Types

- Array

  Conforms when `Element` conforms to `Decodable`.

- Bool
- ClosedRange

  Conforms when `Bound` conforms to `Comparable` and `Decodable`.

- CollectionDifference

  Conforms when `ChangeElement` conforms to `Decodable` and `Encodable`.

- CollectionDifference.Change

  Conforms when `ChangeElement` conforms to `Decodable` and `Encodable`.

- ContiguousArray

  Conforms when `Element` conforms to `Decodable`.

- ContinuousClock.Instant
- Dictionary

  Conforms when `Key` conforms to `Decodable`, `Key` conforms to `Hashable`, and `Value` conforms to `Decodable`.

- Double
- Duration
- Duration.TimeFormatStyle
- Duration.TimeFormatStyle.Attributed
- Duration.TimeFormatStyle.Pattern
- Duration.UnitsFormatStyle
- Duration.UnitsFormatStyle.Attributed
- Duration.UnitsFormatStyle.FractionalPartDisplayStrategy
- Duration.UnitsFormatStyle.Unit
- Duration.UnitsFormatStyle.UnitWidth
- Duration.UnitsFormatStyle.ZeroValueUnitsDisplayStrategy
- Float
- Float16
- Int
- Int128
- Int16
- Int32
- Int64
- Int8
- LocalTestingActorID
- Never
- ObservationRegistrar
- Optional

  Conforms when `Wrapped` conforms to `Decodable`.

- PartialRangeFrom

  Conforms when `Bound` conforms to `Comparable` and `Decodable`.

- PartialRangeThrough

  Conforms when `Bound` conforms to `Comparable` and `Decodable`.

- PartialRangeUpTo

  Conforms when `Bound` conforms to `Comparable` and `Decodable`.

- Range

  Conforms when `Bound` conforms to `Comparable` and `Decodable`.

- SIMD16
- SIMD2
- SIMD3
- SIMD32
- SIMD4
- SIMD64
- SIMD8
- SIMDMask
- Set

  Conforms when `Element` conforms to `Decodable` and `Hashable`.

- String
- String.Comparator
- String.LocalizationValue
- String.LocalizationValue.Placeholder
- String.StandardComparator
- SuspendingClock.Instant
- TaskPriority
- UInt
- UInt128
- UInt16
- UInt32
- UInt64
- UInt8

## See Also

### Custom Encoding and Decoding

Encoding and Decoding Custom Types

Make your data types encodable and decodable for compatibility with external representations such as JSON.

typealias Codable

A type that can convert itself into and out of an external representation.

protocol Encodable

A type that can encode itself to an external representation.

protocol CodingKey

A type that can be used as a key for encoding and decoding.

protocol CodingKeyRepresentable

A type that can be converted to and from a coding key.

struct CodingUserInfoKey

A user-defined key for providing context during encoding and decoding.

