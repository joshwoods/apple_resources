

- Sound Analysis
-  SNTimeDurationConstraint 

Enumeration

# SNTimeDurationConstraint

Defines the time duration windows the request’s underlying sound classifier accepts with a range, or an array, of durations.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum SNTimeDurationConstraint
```

## Topics

### Inspecting a Constraint

case durationRange(CMTimeRange)

A constraint that defines acceptable time window durations with a range.

case enumeratedDurations([CMTime])

A constraint that defines acceptable time window durations in a discrete list.

## See Also

### Inspecting a Request

var knownClassifications: [String]

A string array that contains every prediction label in the request’s underlying sound classifier model.

