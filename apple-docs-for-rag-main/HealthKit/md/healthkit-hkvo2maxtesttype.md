

- HealthKit
-  HKVO2MaxTestType 

Enumeration

# HKVO2MaxTestType

Methods for calculating the user’s VO2 max rate.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 4.0+

``` source
enum HKVO2MaxTestType
```

## Overview

VO2 max represents the maximal oxygen consumption during incremental exercise. VO2 max is an important indicator of fitness and endurance.

## Topics

### Test Types

case maxExercise

A test that measures VO2 max rate by monitoring exercise to the user’s physical limit.

case predictionSubMaxExercise

A calculation that estimates VO2 max rate based on low-intensity exercise.

case predictionNonExercise

A calculation that estimates VO2 max rate without any exercise.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

