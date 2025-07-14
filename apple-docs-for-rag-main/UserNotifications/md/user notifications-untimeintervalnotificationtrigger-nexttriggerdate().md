

- User Notifications
- UNTimeIntervalNotificationTrigger
-  nextTriggerDate() 

Instance Method

# nextTriggerDate()

The next date at which the trigger conditions are met.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func nextTriggerDate() -> Date?
```

## Return Value

The next trigger date.

## Discussion

Use this property to find out when a notification associated with this trigger will next be delivered.

## See Also

### Getting the Trigger Information

var timeInterval: TimeInterval

The time interval to create the trigger.

