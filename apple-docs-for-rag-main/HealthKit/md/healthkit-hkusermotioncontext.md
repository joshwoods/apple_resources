

- HealthKit
-  HKUserMotionContext 

Enumeration

# HKUserMotionContext

The type of motion performed during the sample.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
enum HKUserMotionContext
```

## Topics

### Motion contexts

case notSet

The person’s motion was not specified.

case active

The person was active during the sample.

case stationary

The person was stationary during the sample.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

