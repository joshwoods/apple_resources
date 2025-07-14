

- HealthKit
-  HKAudiogramSample 

Class

# HKAudiogramSample

A sample that stores an audiogram.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class HKAudiogramSample
```

## Overview

This sample stores the results from a hearing test. The sample stores the audiogram data as an array of sensitivity points.

## Topics

### Creating Audiogram Samples

convenience init(sensitivityPoints: [HKAudiogramSensitivityPoint], start: Date, end: Date, metadata: [String : Any]?)

Creates a new audiogram sample.

### Accessing Sensitivity Point Data

var sensitivityPoints: [HKAudiogramSensitivityPoint]

An array of sensitivity point objects.

### Initializers

convenience init(sensitivityPoints: [HKAudiogramSensitivityPoint], start: Date, end: Date, device: HKDevice?, metadata: [String : Any]?)

## Relationships

### Inherits From

- HKSample

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

class HKAudiogramSensitivityPoint

A hearing sensitivity reading associated with a hearing test.

