

- HomeKit
- HMMutableSignificantTimeEvent
-  offset 

Instance Property

# offset

The offset from the significant event that this event fires at.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var offset: DateComponents { get set }
```

## Discussion

To specify that this event should fire before the significant event, supply a date components object with negative values. For example, to specify 30 minutes before sunset, the minute property of the value of the offset property must be set to `-30`.

## See Also

### Configuring a significant time event

var significantEvent: HMSignificantEvent

The significant time-based event that is used to calculate when the event fires.

