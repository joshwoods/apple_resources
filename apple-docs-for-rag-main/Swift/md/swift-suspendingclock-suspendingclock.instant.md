

- Swift
- SuspendingClock
-  SuspendingClock.Instant 

Structure

# SuspendingClock.Instant

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Instant
```

## Topics

### Operators

static func + (SuspendingClock.Instant, Duration) -> SuspendingClock.Instant

static func += (inout SuspendingClock.Instant, Duration)

static func - (SuspendingClock.Instant, Duration) -> SuspendingClock.Instant

static func - (SuspendingClock.Instant, SuspendingClock.Instant) -> Duration

static func -= (inout SuspendingClock.Instant, Duration)

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Type Properties

static var now: SuspendingClock.Instant

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

