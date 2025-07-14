

- EventKit
-  EKCalendarEventAvailabilityMask 

Structure

# EKCalendarEventAvailabilityMask

A bitmask indicating the event availability settings that the calendar can support.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
struct EKCalendarEventAvailabilityMask
```

## Topics

### Initializers

init(rawValue: UInt)

Creates a calendar event availability mask with the specified raw value.

### Type Properties

static var busy: EKCalendarEventAvailabilityMask

The calendar supports the busy event availability setting.

static var free: EKCalendarEventAvailabilityMask

The calendar supports the free event availability setting.

static var tentative: EKCalendarEventAvailabilityMask

The calendar supports the tentative event availability setting.

static var unavailable: EKCalendarEventAvailabilityMask

The calendar supports the unavailable event availability setting.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Accessing Calendar Properties

enum EKCalendarType

Possible calendar types.

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

