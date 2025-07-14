

- EventKit UI
- EKCalendarChooserDelegate
-  calendarChooserDidCancel(\_:) 

Instance Method

# calendarChooserDidCancel(\_:)

Sent when the user cancels a calendar selection.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
optional func calendarChooserDidCancel(_ calendarChooser: EKCalendarChooser)
```

## Parameters 

`calendarChooser`  

The calendar chooser that sent this message.

## See Also

### Selecting Calendars

func calendarChooserDidFinish(EKCalendarChooser)

Sent when a user selects one or more calendars.

func calendarChooserSelectionDidChange(EKCalendarChooser)

Sent when a user changes the selection.

