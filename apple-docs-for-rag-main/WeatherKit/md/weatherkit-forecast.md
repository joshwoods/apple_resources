

- WeatherKit
-  Forecast 

Structure

# Forecast

A forecast collection for minute, hourly, and daily forecasts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Forecast where Element : Decodable, Element : Encodable, Element : Equatable
```

## Overview

Forecast conforms to the `RandomAccessCollection` protocol to support efficient random-access index traversal through forecast types. The protocol involves forwarding the required properties and methods to the underlying forecast collection. The implementation of `subscript` returns an instance of the `Element` type.

## Topics

### Creating the forecast

init(from: any Decoder) throws

init(from: any Decoder) throws

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Serializing objects

func encode(to: any Encoder) throws

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func encode(to: any Encoder) throws

### Getting the properties

var endIndex: Forecast&lt;Element>.Index

The forecast end index.

var forecast: [Element]

The forecast collection.

var metadata: WeatherMetadata

Descriptive information about the forecast data.

var startIndex: Forecast&lt;Element>.Index

The forecast start index.

var summary: String

A convenient localized description of the minute forecast.

### Accessing elements

subscript(Forecast&lt;Element>.Index) -> Element

The forecast element at the provided index.

typealias Index

The forecast index.

### Comparing forecasts

static func == (Forecast&lt;MinuteWeather>, Forecast&lt;MinuteWeather>) -> Bool

### Operators

static func == (Forecast&lt;Element>, Forecast&lt;Element>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Type Aliases

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

## See Also

### Alerts and forecasts

struct WeatherAlert

A weather alert issued for the requested location by a governmental authority.

struct WeatherAvailability

A structure that indicates the availability of data at the requested location.

struct MinuteWeather

A structure that represents the next hour minute forecasts.

struct HourWeather

A structure that represents the weather conditions for the hour.

struct DayWeather

A structure that represents the weather conditions for the day.

