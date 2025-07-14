

- Foundation
- Calendar
-  Calendar.RecurrenceRule 

Structure

# Calendar.RecurrenceRule

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
struct RecurrenceRule
```

## Topics

### Type Aliases

typealias Specification

typealias UnwrappedType

typealias ValueType

### Initializers

init(calendar: Calendar, frequency: Calendar.RecurrenceRule.Frequency, interval: Int, end: Calendar.RecurrenceRule.End, matchingPolicy: Calendar.MatchingPolicy, repeatedTimePolicy: Calendar.RepeatedTimePolicy, months: [Calendar.RecurrenceRule.Month], daysOfTheYear: [Int], daysOfTheMonth: [Int], weeks: [Int], weekdays: [Calendar.RecurrenceRule.Weekday], hours: [Int], minutes: [Int], seconds: [Int], setPositions: [Int])

### Type Properties

static var defaultResolverSpecification: some ResolverSpecification

### Structures

struct End

struct Month

### Instance Properties

var calendar: Calendar

var daysOfTheMonth: [Int]

var daysOfTheYear: [Int]

var end: Calendar.RecurrenceRule.End

var frequency: Calendar.RecurrenceRule.Frequency

var hours: [Int]

var interval: Int

var matchingPolicy: Calendar.MatchingPolicy

var minutes: [Int]

var months: [Calendar.RecurrenceRule.Month]

var repeatedTimePolicy: Calendar.RepeatedTimePolicy

var seconds: [Int]

var setPositions: [Int]

var weekdays: [Calendar.RecurrenceRule.Weekday]

var weeks: [Int]

### Instance Methods

func recurrences(of: Date, in: Range&lt;Date>?) -> some Sendable &amp; Sequence&lt;Date> 

### Type Methods

static func daily(calendar: Calendar, interval: Int, end: Calendar.RecurrenceRule.End, matchingPolicy: Calendar.MatchingPolicy, repeatedTimePolicy: Calendar.RepeatedTimePolicy, months: [Calendar.RecurrenceRule.Month], daysOfTheMonth: [Int], weekdays: [Calendar.RecurrenceRule.Weekday], hours: [Int], minutes: [Int], seconds: [Int], setPositions: [Int]) -> Calendar.RecurrenceRule

static func hourly(calendar: Calendar, interval: Int, end: Calendar.RecurrenceRule.End, matchingPolicy: Calendar.MatchingPolicy, repeatedTimePolicy: Calendar.RepeatedTimePolicy, months: [Calendar.RecurrenceRule.Month], daysOfTheYear: [Int], daysOfTheMonth: [Int], weekdays: [Calendar.RecurrenceRule.Weekday], hours: [Int], minutes: [Int], seconds: [Int], setPositions: [Int]) -> Calendar.RecurrenceRule

static func minutely(calendar: Calendar, interval: Int, end: Calendar.RecurrenceRule.End, matchingPolicy: Calendar.MatchingPolicy, repeatedTimePolicy: Calendar.RepeatedTimePolicy, months: [Calendar.RecurrenceRule.Month], daysOfTheYear: [Int], daysOfTheMonth: [Int], weekdays: [Calendar.RecurrenceRule.Weekday], hours: [Int], minutes: [Int], seconds: [Int], setPositions: [Int]) -> Calendar.RecurrenceRule

static func monthly(calendar: Calendar, interval: Int, end: Calendar.RecurrenceRule.End, matchingPolicy: Calendar.MatchingPolicy, repeatedTimePolicy: Calendar.RepeatedTimePolicy, months: [Calendar.RecurrenceRule.Month], daysOfTheMonth: [Int], weekdays: [Calendar.RecurrenceRule.Weekday], hours: [Int], minutes: [Int], seconds: [Int], setPositions: [Int]) -> Calendar.RecurrenceRule

static func weekly(calendar: Calendar, interval: Int, end: Calendar.RecurrenceRule.End, matchingPolicy: Calendar.MatchingPolicy, repeatedTimePolicy: Calendar.RepeatedTimePolicy, months: [Calendar.RecurrenceRule.Month], weekdays: [Calendar.RecurrenceRule.Weekday], hours: [Int], minutes: [Int], seconds: [Int], setPositions: [Int]) -> Calendar.RecurrenceRule

static func yearly(calendar: Calendar, interval: Int, end: Calendar.RecurrenceRule.End, matchingPolicy: Calendar.MatchingPolicy, repeatedTimePolicy: Calendar.RepeatedTimePolicy, months: [Calendar.RecurrenceRule.Month], daysOfTheYear: [Int], daysOfTheMonth: [Int], weeks: [Int], weekdays: [Calendar.RecurrenceRule.Weekday], hours: [Int], minutes: [Int], seconds: [Int], setPositions: [Int]) -> Calendar.RecurrenceRule

### Enumerations

enum Frequency

enum Weekday

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

