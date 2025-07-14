

- User Notifications
- UNCalendarNotificationTrigger
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

Use this property to find out when the system will deliver a notification associated with this trigger.

## See Also

### Getting the Trigger Information

var dateComponents: DateComponents

The date components to construct this object.

