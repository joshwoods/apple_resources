

- EventKit UI
-  EKCalendarChooserSelectionStyle 

Enumeration

# EKCalendarChooserSelectionStyle

Indicates whether users may select a single calendar, or multiple calendars.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
enum EKCalendarChooserSelectionStyle
```

## Topics

### Constants

case single

A style that limits users to selecting a single calendar.

case multiple

A style that lets users select multiple calendars.

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

enum EKCalendarChooserDisplayStyle

Indicates whether to display all calendars or writable calendars only.

