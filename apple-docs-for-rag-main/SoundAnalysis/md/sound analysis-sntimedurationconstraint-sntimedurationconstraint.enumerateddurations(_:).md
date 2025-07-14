

- Sound Analysis
- SNTimeDurationConstraint
-  SNTimeDurationConstraint.enumeratedDurations(\_:) 

Case

# SNTimeDurationConstraint.enumeratedDurations(\_:)

A constraint that defines acceptable time window durations in a discrete list.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
case enumeratedDurations([CMTime])
```

## Parameters 

`timeDurations`  

An array of time durations the request’s underlying sound classifier accepts.

## See Also

### Inspecting a Constraint

case durationRange(CMTimeRange)

A constraint that defines acceptable time window durations with a range.

