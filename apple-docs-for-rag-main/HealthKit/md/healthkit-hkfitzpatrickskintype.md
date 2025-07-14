

- HealthKit
-  HKFitzpatrickSkinType 

Enumeration

# HKFitzpatrickSkinType

Categories representing the user’s skin type based on the Fitzpatrick scale.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
enum HKFitzpatrickSkinType
```

## Overview

The Fitzpatrick scale is a numerical classification for skin color based on the skins response to sun exposure in terms of the degree of burning and tanning.

## Topics

### Constants

case notSet

Either the user’s skin type is not set, or the user has not granted your app permission to read the skin type.

case I

Pale white skin that always burns easily in the sun and never tans.

case II

White skin that burns easily and tans minimally.

case III

White to light brown skin that burns moderately and tans uniformly.

case IV

Beige-olive, lightly tanned skin that burns minimally and tans moderately.

case V

Brown skin that rarely burns and tans profusely.

case VI

Dark brown to black skin that never burns and tans profusely.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

enum HKAudiogramConductionType

enum HKAudiogramSensitivityTestSide

enum HKCategoryValueVaginalBleeding

enum Answer

enum Risk

enum Answer

enum Risk

enum Association

enum Kind

enum Label

enum ValenceClassification

enum HKWorkoutEffortRelationshipQueryOptions

enum HKBiologicalSex

Constants indicating the user’s sex.

enum HKBloodType

Constants indicating the user’s blood type.

enum HKWheelchairUse

Constants indicating the user’s wheelchair use.

