

- EventKit
- EKCalendar
-  type 

Instance Property

# type

The calendar’s type.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 2.0+

``` source
var type: EKCalendarType { get }
```

## Discussion

CalDAV-subscribed calendars are of type EKCalendarType.calDAV with isSubscribed set to true.

## See Also

### Accessing Calendar Properties

enum EKCalendarType

Possible calendar types.

struct EKCalendarEventAvailabilityMask

A bitmask indicating the event availability settings that the calendar can support.

var allowsContentModifications: Bool

A Boolean value that indicates whether you can add, edit, and delete items in the calendar.

var cgColor: CGColor!

The calendar’s color.

var color: NSColor!

The calendar’s color.

var isImmutable: Bool

A Boolean value indicating whether the calendar’s properties can be edited or deleted.

var title: String

The calendar’s title.

var allowedEntityTypes: EKEntityMask

The entity types this calendar can contain.

var source: EKSource!

The source object representing the account to which this calendar belongs.

var isSubscribed: Bool

A Boolean value indicating whether the calendar is a subscribed calendar.

var supportedEventAvailabilities: EKCalendarEventAvailabilityMask

The event availability settings supported by this calendar, as indicated by a bitmask.

var calendarIdentifier: String

A unique identifier for the calendar.

func DATETIME_COMPONENTS_DO_NOT_USE()

A deprecated function.

Deprecated

func DATE_COMPONENTS_DO_NOT_USE()

A deprecated function.

Deprecated

