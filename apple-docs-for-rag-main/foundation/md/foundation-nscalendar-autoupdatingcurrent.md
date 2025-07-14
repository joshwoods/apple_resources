

- Foundation
- NSCalendar
-  autoupdatingCurrent 

Type Property

# autoupdatingCurrent

A calendar that tracks changes to user’s preferred calendar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var autoupdatingCurrent: Calendar { get }
```

## Return Value

The current logical calendar for the current user.

## Discussion

Settings you get from this calendar do change as the user’s settings change (contrast with current).

Note that if you cache values based on the calendar or related information those caches will of course not be automatically updated by the updating of the calendar object.

## See Also

### Related Documentation

init?(calendarIdentifier: NSCalendar.Identifier)

Initializes a calendar according to a given identifier.

var calendarIdentifier: NSCalendar.Identifier

An identifier for the calendar.

### Getting the User’s Calendar

class var current: Calendar

The user’s current calendar.

