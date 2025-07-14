

- EventKit UI
- EKCalendarChooserDelegate
-  calendarChooserSelectionDidChange(\_:) 

Instance Method

# calendarChooserSelectionDidChange(\_:)

Sent when a user changes the selection.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
optional func calendarChooserSelectionDidChange(_ calendarChooser: EKCalendarChooser)
```

## Parameters 

`calendarChooser`  

The calendar chooser that sent this message.

## Discussion

Use the selectedCalendars property to get the current selection.

## See Also

### Selecting Calendars

func calendarChooserDidFinish(EKCalendarChooser)

Sent when a user selects one or more calendars.

func calendarChooserDidCancel(EKCalendarChooser)

Sent when the user cancels a calendar selection.

