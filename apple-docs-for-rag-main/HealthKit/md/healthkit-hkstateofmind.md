

- HealthKit
-  HKStateOfMind 

Class

# HKStateOfMind

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+watchOS 11.0+

``` source
class HKStateOfMind
```

## Topics

### Initializers

convenience init(date: Date, kind: HKStateOfMind.Kind, valence: Double, labels: [HKStateOfMind.Label], associations: [HKStateOfMind.Association], metadata: [String : Any]?)

### Instance Properties

var associations: [HKStateOfMind.Association]

var kind: HKStateOfMind.Kind

var labels: [HKStateOfMind.Label]

var valence: Double

var valenceClassification: HKStateOfMind.ValenceClassification

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Classes

class HKAudiogramSensitivityPointClampingRange

Defines the range within which an ear’s sensitivity point may have been clamped, if any.

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

class HKStateOfMindType

class HKWheelchairUseObject

This class acts as a wrapper for the wheelchair use enumeration.

class HKWorkoutEffortRelationship

class HKWorkoutEffortRelationshipQuery

