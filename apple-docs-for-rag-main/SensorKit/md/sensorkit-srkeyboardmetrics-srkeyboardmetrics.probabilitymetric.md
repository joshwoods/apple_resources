

- SensorKit
- SRKeyboardMetrics
-  SRKeyboardMetrics.ProbabilityMetric 

Class

# SRKeyboardMetrics.ProbabilityMetric

A likelihood of occurrence.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class ProbabilityMetric where UnitType : Unit
```

## Overview

The framework derives these values based on raw sensor data.

## Topics

### Sample Values

var distributionSampleValues: [Measurement&lt;UnitType>]

An array of sample values from the probability distribution.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Timing Key Use

var touchDownUp: ProbabilityMetric&lt;UnitDuration>

The duration between touch down to touch up for any key.

var touchUpDown: ProbabilityMetric&lt;UnitDuration>

The duration between touch up and touch down for any key.

var spaceTouchDownUp: ProbabilityMetric&lt;UnitDuration>

The duration between touch down and touch up of all Space bar events for the keyboard.

var deleteTouchDownUp: ProbabilityMetric&lt;UnitDuration>

The duration between touch down and touch up of all Delete key events for the keyboard.

var shortWordCharKeyTouchDownUp: ProbabilityMetric&lt;UnitDuration>

The duration between touch down and touch up of all character keys in short words for the keyboard.

var touchDownDown: ProbabilityMetric&lt;UnitDuration>

The duration between touch down and touch down for any key.

var charKeyToPrediction: ProbabilityMetric&lt;UnitDuration>

The duration between touch up on a character key and touch down on a word in the prediction bar.

var shortWordCharKeyToCharKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up on a character key and touch down on any sequential character key in a short word.

var charKeyToAnyTapKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up on a character key and touch down on the next sequential key.

var anyTapToCharKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of any key and touch down on a sequential character key.

var spaceToCharKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Space bar and touch down of a sequential character key.

var charKeyToSpaceKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of a character key and touch down of a sequential Space bar.

var spaceToDeleteKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Space bar and touch down of a sequential Delete key.

var deleteToSpaceKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Delete key and touch down of a sequential Space bar.

var spaceToSpaceKey: ProbabilityMetric&lt;UnitDuration>

The duration between touch up of the Space bar and touch down of a sequential Space bar.

