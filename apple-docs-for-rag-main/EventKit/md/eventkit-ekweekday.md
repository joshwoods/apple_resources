

- EventKit
-  EKWeekday 

Enumeration

# EKWeekday

The day of the week.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
@frozen
enum EKWeekday
```

## Topics

### Constants

case sunday

The value for Sunday.

case monday

The value for Monday.

case tuesday

The value for Tuesday.

case wednesday

The value for Wednesday.

case thursday

The value for Thursday.

case friday

The value for Friday.

case saturday

The value for Saturday.

### Deprecated

static var EKSunday: EKWeekday

The value for Sunday.

Deprecated

static var EKMonday: EKWeekday

The value for Monday.

Deprecated

static var EKTuesday: EKWeekday

The value for Tuesday.

Deprecated

static var EKWednesday: EKWeekday

The value for Wednesday.

Deprecated

static var EKThursday: EKWeekday

The value for Thursday.

Deprecated

static var EKFriday: EKWeekday

The value for Friday.

Deprecated

static var EKSaturday: EKWeekday

The value for Saturday.

Deprecated

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

### Creating a Day of the Week

convenience init(EKWeekday)

Creates and returns a day of the week with a given day.

convenience init(EKWeekday, weekNumber: Int)

Creates and returns an autoreleased day of the week with a given day and week number.

init(dayOfTheWeek: EKWeekday, weekNumber: Int)

Initializes and returns a day of the week with a given day and week number.

