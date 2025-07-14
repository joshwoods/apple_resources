

- HomeKit
-  HMSignificantEvent 

Structure

# HMSignificantEvent

An event that represents significant time-based events, including sunrise and sunset.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
struct HMSignificantEvent
```

## Topics

### Significant event properties

static let sunrise: HMSignificantEvent

An event that fires at sunrise.

static let sunset: HMSignificantEvent

An event that fires at sunset.

### Creating a significant event

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Significant events

class HMSignificantTimeEvent

An event that fires at a time offset from a significant time-based event.

class HMMutableSignificantTimeEvent

A mutable event that fires at the specified temporal offset to a significant event.

