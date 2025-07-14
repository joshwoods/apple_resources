

- EventKit UI
-  EKCalendarChooserDelegate 

Protocol

# EKCalendarChooserDelegate

Methods a calendar chooser’s delegate may use to receive notifications.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
protocol EKCalendarChooserDelegate : NSObjectProtocol
```

## Topics

### Selecting Calendars

func calendarChooserDidFinish(EKCalendarChooser)

Sent when a user selects one or more calendars.

func calendarChooserSelectionDidChange(EKCalendarChooser)

Sent when a user changes the selection.

func calendarChooserDidCancel(EKCalendarChooser)

Sent when the user cancels a calendar selection.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Managing Calendar Selection

var delegate: (any EKCalendarChooserDelegate)?

The calendar chooser’s delegate.

