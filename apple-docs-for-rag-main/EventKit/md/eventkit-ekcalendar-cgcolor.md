

- EventKit
- EKCalendar
-  cgColor 

Instance Property

# cgColor

The calendar’s color.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
var cgColor: CGColor! { get set }
```

## Discussion

This property is the equivalent of the color property in macOS.

## See Also

### Accessing Calendar Properties

enum EKCalendarType

Possible calendar types.

struct EKCalendarEventAvailabilityMask

A bitmask indicating the event availability settings that the calendar can support.

var allowsContentModifications: Bool

A Boolean value that indicates whether you can add, edit, and delete items in the calendar.

var color: NSColor!

The calendar’s color.

var isImmutable: Bool

A Boolean value indicating whether the calendar’s properties can be edited or deleted.

var title: String

The calendar’s title.

var type: EKCalendarType

The calendar’s type.

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

