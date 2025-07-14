

- HomeKit
- HMEventTrigger
-  endEvents 

Instance Property

# endEvents

The events associated with the end of scene represented by this trigger.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var endEvents: [HMEvent] { get }
```

## Discussion

HomeKit restores the previously active scene when the events in this array trigger. For example, you can use end events to execute a scene for 10 minutes by specifying an HMDurationEvent in the list of endEvents. This restores the previous scene when the duration event triggers.

You can also use HMCharacteristicEvent and HMCharacteristicThresholdRangeEvent objects as end events.

## See Also

### Restoring the previous scene after an event

func updateEndEvents([HMEvent], completionHandler: ((any Error)?) -> Void)

Updates the set of end events associated with the event trigger.

