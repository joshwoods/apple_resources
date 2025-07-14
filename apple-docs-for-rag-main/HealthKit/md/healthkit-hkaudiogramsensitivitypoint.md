

- HealthKit
-  HKAudiogramSensitivityPoint 

Class

# HKAudiogramSensitivityPoint

A hearing sensitivity reading associated with a hearing test.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class HKAudiogramSensitivityPoint
```

## Topics

### Creating Sensitivity Points

convenience init(frequency: HKQuantity, leftEarSensitivity: HKQuantity?, rightEarSensitivity: HKQuantity?) throws

Creates a new sensitivity point.

Deprecated

### Accessing Data

var frequency: HKQuantity

The frequency tested in the hearing test.

var leftEarSensitivity: HKQuantity?

The sensitivity of the left ear.

Deprecated

var rightEarSensitivity: HKQuantity?

The sensitivity of the right ear.

Deprecated

### Initializers

convenience init(frequency: HKQuantity, tests: [HKAudiogramSensitivityTest]) throws

### Instance Properties

var tests: [HKAudiogramSensitivityTest]

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Audiograms

class HKAudiogramSample

A sample that stores an audiogram.

