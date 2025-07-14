

- Foundation
-  DiscreteFormatStyle 

Protocol

# DiscreteFormatStyle

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
protocol DiscreteFormatStyle : FormatStyle
```

## Topics

### Instance Methods

func discreteInput(after: Self.FormatInput) -> Self.FormatInput?

**Required**

func discreteInput(before: Self.FormatInput) -> Self.FormatInput?

**Required**

func input(after: Self.FormatInput) -> Self.FormatInput?

**Required** Default implementations provided.

func input(before: Self.FormatInput) -> Self.FormatInput?

**Required** Default implementations provided.

## Relationships

### Inherits From

- Decodable
- Encodable
- Equatable
- FormatStyle
- Hashable

### Conforming Types

- Date.AnchoredRelativeFormatStyle
- Date.ComponentsFormatStyle
- Date.FormatStyle
- Date.FormatStyle.Attributed
- Date.VerbatimFormatStyle
- Date.VerbatimFormatStyle.Attributed

## See Also

### Protocols

protocol NSKeyValueObservingCustomization

Conforming to NSKeyValueObservingCustomization is not required to use Key-Value Observing. Provide an implementation of these functions if you need to disable auto-notifying for a key, or add dependent keys

