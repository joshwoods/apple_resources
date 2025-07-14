

- Swift
- ContinuousClock
-  ContinuousClock.Instant 

Structure

# ContinuousClock.Instant

A continuous point in time used for `ContinuousClock`.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Instant
```

## Topics

### Operators

static func + (ContinuousClock.Instant, Duration) -> ContinuousClock.Instant

static func += (inout ContinuousClock.Instant, Duration)

static func - (ContinuousClock.Instant, ContinuousClock.Instant) -> Duration

static func - (ContinuousClock.Instant, Duration) -> ContinuousClock.Instant

static func -= (inout ContinuousClock.Instant, Duration)

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Type Properties

static var now: ContinuousClock.Instant

### Default Implementations

Comparable Implementations

Equatable Implementations

Hashable Implementations

InstantProtocol Implementations

## Relationships

### Conforms To

- Comparable
- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- InstantProtocol
- Sendable

