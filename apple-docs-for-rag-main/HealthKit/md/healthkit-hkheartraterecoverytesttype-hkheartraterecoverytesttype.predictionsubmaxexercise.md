

- HealthKit
- HKHeartRateRecoveryTestType
-  HKHeartRateRecoveryTestType.predictionSubMaxExercise 

Case

# HKHeartRateRecoveryTestType.predictionSubMaxExercise

A test that estimates a person’s heart-rate recovery using lower-intensity exercise.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
case predictionSubMaxExercise
```

## Discussion

In this test, a person performs lower-intensity exercise, staying below their physical limit. The test then estimates their actual heart rate recovery based on the difference between their exercising heart rate, and the rate of recovery after the exercise ends.

## See Also

### Heart-rate recovery tests

case maxExercise

Measures a person’s actual heart-rate recovery.

case predictionNonExercise

A test that estimates a person’s heart-rate recovery without using exercise.

