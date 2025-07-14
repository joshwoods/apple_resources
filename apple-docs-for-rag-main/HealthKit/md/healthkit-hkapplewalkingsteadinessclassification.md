

- HealthKit
-  HKAppleWalkingSteadinessClassification 

Enumeration

# HKAppleWalkingSteadinessClassification

A classification of a score based on the steadiness of the user’s gait.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+visionOS 1.0+watchOS 8.0+

``` source
enum HKAppleWalkingSteadinessClassification
```

## Overview

Walking Steadiness classifications measures the ability of the user to move with a steady, even gait. You can use the HKAppleWalkingSteadinessClassificationForQuantity, HKAppleWalkingSteadinessMaximumQuantityForClassification, and HKAppleWalkingSteadinessMinimumQuantityForClassification methods to convert between Walking Steadiness scores and the HKAppleWalkingSteadinessClassification.low, HKAppleWalkingSteadinessClassification.veryLow, or HKAppleWalkingSteadinessClassification.ok classifications.

## Topics

### Accessing Classifications

case ok

A classification indicating that the stability of the user’s gait is within the normal range.

case low

A classification indicating that the stability of the user’s gate is below normal.

case veryLow

A classification indicating that the stability of the user’s gate is considerably below normal.

### Initializers

init(for: HKQuantity) throws

Creates a new classification for the provided percentage.

init?(rawValue: Int)

### Instance Properties

var maximum: HKQuantity

The minimum walking steadiness percentage for the classification.

var minimum: HKQuantity

The maximum walking steadiness percentage for the classification.

### Default Implementations

CaseIterable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- CaseIterable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

