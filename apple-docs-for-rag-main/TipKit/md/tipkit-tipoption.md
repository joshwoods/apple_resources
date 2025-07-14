

- TipKit
-  TipOption 

Protocol

# TipOption

A type that represents the various customizations that you can make to a tip’s behavior.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol TipOption : Sendable
```

## Topics

### Tip options

typealias IgnoresDisplayFrequency

Controls whether a tip obeys the preconfigured display frequency interval.

typealias MaxDisplayCount

Specifies the maximum number of times a tip displays before the system automatically invalidates it.

typealias MaxDisplayDuration

Specifies the maximum amount of time a tip is displayed before it is invalidated.

## Relationships

### Inherits From

- Sendable

### Conforming Types

- Tips.IgnoresDisplayFrequency
- Tips.MaxDisplayCount
- Tips.MaxDisplayDuration

## See Also

### Common types

struct AnyTip

A type-erased tip value.

