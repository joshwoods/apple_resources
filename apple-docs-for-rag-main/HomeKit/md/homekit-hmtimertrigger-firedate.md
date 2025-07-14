

- HomeKit
- HMTimerTrigger
-  fireDate 

Instance Property

# fireDate

The time at which the trigger will next fire.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var fireDate: Date { get }
```

## Discussion

Timer triggers are only set at the beginning of a minute. Seconds are not used and an error will be returned if the fire date includes a seconds value other than 0. When the timer fires, it will typically fire within 1 minute of the scheduled fire date or calculated recurrence fire date, depending on system power and resource management.

## See Also

### Choosing the fire date

func updateFireDate(Date, completionHandler: ((any Error)?) -> Void)

Updates the next fire date for the trigger.

