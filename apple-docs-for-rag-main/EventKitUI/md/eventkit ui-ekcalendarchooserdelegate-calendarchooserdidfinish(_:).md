

- EventKit UI
- EKCalendarChooserDelegate
-  calendarChooserDidFinish(\_:) 

Instance Method

# calendarChooserDidFinish(\_:)

Sent when a user selects one or more calendars.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
optional func calendarChooserDidFinish(_ calendarChooser: EKCalendarChooser)
```

## Parameters 

`calendarChooser`  

The calendar chooser that sent this message.

## See Also

### Selecting Calendars

func calendarChooserSelectionDidChange(EKCalendarChooser)

Sent when a user changes the selection.

func calendarChooserDidCancel(EKCalendarChooser)

Sent when the user cancels a calendar selection.

