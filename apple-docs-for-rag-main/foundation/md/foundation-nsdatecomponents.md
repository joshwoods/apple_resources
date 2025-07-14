

- Foundation
-  NSDateComponents 

Class

# NSDateComponents

An object that specifies a date or time in terms of units (such as year, month, day, hour, and minute) to be evaluated in a calendar system and time zone.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSDateComponents
```

## Overview

In Swift, this object bridges to DateComponents; use NSDateComponents when you need reference semantics or other Foundation-specific behavior.

NSDateComponents encapsulates the components of a date in an extendable, object-oriented manner. It’s used to specify a date by providing the temporal components that make up a date and time: hour, minutes, seconds, day, month, year, and so on. You can also use it to specify a duration of time, for example, 5 hours and 16 minutes. An NSDateComponents object is not required to define all the component fields. When a new instance of NSDateComponents is created, the date components are set to NSDateComponentUndefined.

Important

An NSDateComponents object is meaningless in itself; you need to know what calendar it is interpreted against, and you need to know whether the values are absolute values of the units, or quantities of the units.

An instance of NSDateComponents is not responsible for answering questions about a date beyond the information with which it was initialized. For example, if you initialize one with May 4, 2017, its weekday is NSDateComponentUndefined, not Thursday. To get the correct day of the week, you must create a suitable instance of NSCalendar, create an NSDate object using date(from:) and then use components(_:from:) to retrieve the weekday—as illustrated in the following example.

- Swift
- Objective-C

```
let dateComponents = NSDateComponents()
dateComponents.day = 4
dateComponents.month = 5
dateComponents.year = 2017

if let gregorianCalendar = NSCalendar(calendarIdentifier: .gregorian),
    let date = gregorianCalendar.date(from: dateComponents as DateComponents) {
    let weekday = gregorianCalendar.component(.weekday, from: date)
    print(weekday) // 5, which corresponds to Thursday in the Gregorian Calendar
}

```

```
NSDateComponents *dateComponents = [[NSDateComponents alloc] init];
dateComponents.day = 4;
dateComponents.month = 5;
dateComponents.year = 2017;

NSCalendar *gregorianCalendar = [[NSCalendar alloc] initWithCalendarIdentifier:NSCalendarIdentifierGregorian];
NSDate *date = [gregorianCalendar dateFromComponents:dateComponents];

NSInteger weekday = [gregorianCalendar component:NSCalendarUnitWeekday fromDate:date];
NSLog(@"%d", weekday); // 5, which corresponds to Thursday in the Gregorian Calendar
```

For more details, see Calendars, Date Components, and Calendar Units in Date and Time Programming Guide.

Important

The Swift overlay to the Foundation framework provides the DateComponents structure, which bridges to the NSDateComponents class. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Setting a Calendar and Time Zone

var calendar: Calendar?

The calendar used to interpret the date components.

var timeZone: TimeZone?

The time zone used to interpret the date components.

### Validating a Date

var isValidDate: Bool

A Boolean value that indicates whether the current combination of properties represents a date which exists in the current calendar.

func isValidDate(in: Calendar) -> Bool

Returns a Boolean value that indicates whether the current combination of properties represents a date which exists in the specified calendar.

var date: Date?

The date calculated from the current components using the stored calendar.

Undefined Components

Constants that denote that the value of a date component is undefined.

### Accessing Years and Months

var era: Int

The number of eras.

var year: Int

The number of years.

var yearForWeekOfYear: Int

The ISO 8601 week-numbering year.

var quarter: Int

The number of quarters.

var month: Int

The number of months.

var isLeapMonth: Bool

A Boolean value that indicates whether the month is a leap month.

### Accessing Weeks and Days

var weekday: Int

The number of the weekdays.

var weekdayOrdinal: Int

The ordinal number of weekdays.

var weekOfMonth: Int

The week number of the months.

var weekOfYear: Int

The ISO 8601 week date of the year.

var day: Int

The number of days.

func week() -> Int

Returns the number of weeks.

Deprecated

func setWeek(Int)

Sets the number of weeks.

Deprecated

### Accessing Hours and Seconds

var hour: Int

The number of hour units for the receiver.

var minute: Int

The number of minute units for the receiver.

var second: Int

The number of second units for the receiver.

var nanosecond: Int

The number of nanosecond units for the receiver.

### Accessing Components as Calendrical Units

func value(forComponent: NSCalendar.Unit) -> Int

Returns the value for a given calendar unit.

func setValue(Int, forComponent: NSCalendar.Unit)

Sets a value for a given calendar unit.

struct Unit

Calendrical units such as year, month, day and hour.

### Instance Properties

var dayOfYear: Int

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

