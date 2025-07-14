

- EventKit UI
- EKEventEditViewDelegate
-  eventEditViewControllerDefaultCalendar(forNewEvents:) 

Instance Method

# eventEditViewControllerDefaultCalendar(forNewEvents:)

The default calendar to use when creating new events.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
optional func eventEditViewControllerDefaultCalendar(forNewEvents controller: EKEventEditViewController) -> EKCalendar
```

## Parameters 

`controller`  

The event edit view controller requesting the default calendar.

## Discussion

If the delegate does not implement this method, uses the event store’s defaultCalendarForNewEvents property instead.

