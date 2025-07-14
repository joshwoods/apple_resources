

- User Notifications
- UNTimeIntervalNotificationTrigger
-  timeInterval 

Instance Property

# timeInterval

The time interval to create the trigger.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var timeInterval: TimeInterval { get }
```

## Discussion

This property contains the original time interval that you specified when creating the trigger object. The value in this property isn’t updated as time counts down. To find out when the trigger will fire next, call the nextTriggerDate() method.

## See Also

### Getting the Trigger Information

func nextTriggerDate() -> Date?

The next date at which the trigger conditions are met.

