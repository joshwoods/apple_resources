

- Sound Analysis
- SNClassifySoundRequest
-  windowDurationConstraint 

Instance Property

# windowDurationConstraint

A range or list of sound duration times the request’s underlying sound classifier supports.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@nonobjc
var windowDurationConstraint: SNTimeDurationConstraint { get }
```

## Discussion

Configure the request’s windowDuration property with a value that satisfies the window duration constraint.

