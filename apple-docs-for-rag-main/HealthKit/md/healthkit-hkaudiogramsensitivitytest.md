

- HealthKit
-  HKAudiogramSensitivityTest 

Class

# HKAudiogramSensitivityTest

iOS 18.1+iPadOS 18.1+Mac Catalyst 18.1+macOS 15.1+visionOS 2.1+watchOS 11.1+

``` source
class HKAudiogramSensitivityTest
```

## Topics

### Initializers

init(sensitivity: HKQuantity, type: HKAudiogramConductionType, masked: Bool, side: HKAudiogramSensitivityTestSide, clampingRange: HKAudiogramSensitivityPointClampingRange?) throws

### Instance Properties

var clampingRange: HKAudiogramSensitivityPointClampingRange?

var masked: Bool

var sensitivity: HKQuantity

var side: HKAudiogramSensitivityTestSide

var type: HKAudiogramConductionType

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

class HKAudiogramSensitivityPointClampingRange

Defines the range within which an ear’s sensitivity point may have been clamped, if any.

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

