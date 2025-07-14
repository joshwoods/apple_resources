

- EventKit UI
-  EKCalendarChooserDisplayStyle 

Enumeration

# EKCalendarChooserDisplayStyle

Indicates whether to display all calendars or writable calendars only.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
enum EKCalendarChooserDisplayStyle
```

## Topics

### Constants

case allCalendars

Displays writable and read-only calendars.

case writableCalendarsOnly

Displays writable calendars only.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Selecting a Calendar Type

var selectedCalendars: Set&lt;EKCalendar>

The calendars selected by the user.

var selectionStyle: EKCalendarChooserSelectionStyle

Determines whether to allow selection of multiple calendars.

enum EKCalendarChooserSelectionStyle

Indicates whether users may select a single calendar, or multiple calendars.

