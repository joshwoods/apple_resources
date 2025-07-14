

- WeatherKit
-  TrendBaseline 

Structure

# TrendBaseline

A type encapsulating everything there is to know about what a trend baseline is.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct TrendBaseline where Dimension : Dimension
```

## Topics

### Operators

static func == (TrendBaseline&lt;Dimension>, TrendBaseline&lt;Dimension>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

let kind: TrendBaseline&lt;Dimension>.Kind

The manner in which the comparison between the baseline and current values are compared.

let startDate: Date

The year the statistics collection began.

let value: Measurement&lt;Dimension>

The recorded baseline value for the condition in which the trend is comparing to.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Enumerations

enum Kind

An enum describing what value is being compared between historical and current readings.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable

