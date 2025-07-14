

- WeatherKit
- UVIndex
-  UVIndex.ExposureCategory 

Enumeration

# UVIndex.ExposureCategory

An enumeration that indicates risk of harm from unprotected sun exposure.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
enum ExposureCategory
```

## Topics

### Operators

static func &lt; (UVIndex.ExposureCategory, UVIndex.ExposureCategory) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

### Enumeration Cases

case extreme

The UV index is extreme.

case high

The UV index is high.

case low

The UV index is low.

case moderate

The UV index is moderate.

case veryHigh

The UV index is very high.

### Initializers

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var accessibilityDescription: String

A localized accessibility description describing the UV Index Exposure Category.

var description: String

A localized string describing the risk of harm from unprotected sun exposure.

var rangeValue: ClosedRange&lt;Int>

The range of UV index values that falls into this category.

var rawValue: String

The corresponding value of the raw type.

### Type Aliases

typealias AllCases

A type that can represent a collection of all values of this type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static var allCases: [UVIndex.ExposureCategory]

A collection of all values of this type.

### Default Implementations

Comparable Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- CaseIterable
- Comparable
- Copyable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the UV index

var category: UVIndex.ExposureCategory

The UV Index exposure category.

var value: Int

The UV Index value.

