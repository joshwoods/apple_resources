

- HealthKit
-  HKAudiogramSensitivityPointClampingRange 

Class

# HKAudiogramSensitivityPointClampingRange

Defines the range within which an ear’s sensitivity point may have been clamped, if any.

iOS 18.1+iPadOS 18.1+Mac Catalyst 18.1+macOS 15.1+visionOS 2.1+watchOS 11.1+

``` source
class HKAudiogramSensitivityPointClampingRange
```

## Overview

At times, it may be required to indicate that a sensitivity point has been clamped to a range. These reasons include but are not limited to user safety, hardware limitations, or algorithm features.

## Topics

### Initializers

convenience init(lowerBound: NSNumber?, upperBound: NSNumber?) throws

### Instance Properties

var lowerBound: HKQuantity?

var upperBound: HKQuantity?

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Classes

class HKAudiogramSensitivityTest

class HKBiologicalSexObject

This class acts as a wrapper for the HKBiologicalSex enumeration.

class HKBloodTypeObject

This class acts as a wrapper for the HKBloodType enumeration.

class HKFitzpatrickSkinTypeObject

This class acts as a wrapper for the HKFitzpatrickSkinType enumeration.

class HKGAD7Assessment

class HKPHQ9Assessment

class HKScoredAssessment

class HKScoredAssessmentType

class HKStateOfMind

class HKStateOfMindType

class HKWheelchairUseObject

This class acts as a wrapper for the wheelchair use enumeration.

class HKWorkoutEffortRelationship

class HKWorkoutEffortRelationshipQuery

