

- Foundation
- NSCalendar
-  current 

Type Property

# current

The user’s current calendar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var current: Calendar { get }
```

## Return Value

The logical calendar for the current user.

## Discussion

The returned calendar is formed from the settings for the current user’s chosen system locale overlaid with any custom settings the user has specified in System Preferences. Settings you get from this calendar do not change as System Preferences are changed, so that your operations are consistent (contrast with autoupdatingCurrent).

## See Also

### Related Documentation

Date and Time Programming Guide

Data Formatting Guide

init?(calendarIdentifier: NSCalendar.Identifier)

Initializes a calendar according to a given identifier.

var calendarIdentifier: NSCalendar.Identifier

An identifier for the calendar.

### Getting the User’s Calendar

class var autoupdatingCurrent: Calendar

A calendar that tracks changes to user’s preferred calendar.

