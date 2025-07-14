

- EventKit UI
- EKCalendarChooser
-  selectionStyle 

Instance Property

# selectionStyle

Determines whether to allow selection of multiple calendars.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
@MainActor
var selectionStyle: EKCalendarChooserSelectionStyle { get }
```

## Discussion

Possible values are described in EKCalendarChooserSelectionStyle.

## See Also

### Selecting a Calendar Type

var selectedCalendars: Set&lt;EKCalendar>

The calendars selected by the user.

enum EKCalendarChooserSelectionStyle

Indicates whether users may select a single calendar, or multiple calendars.

enum EKCalendarChooserDisplayStyle

Indicates whether to display all calendars or writable calendars only.

