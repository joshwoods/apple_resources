

- Foundation
- NSCalendar
-  init(identifier:) 

Initializer

# init(identifier:)

Creates a new calendar specified by a given identifier.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(identifier calendarIdentifierConstant: NSCalendar.Identifier)
```

## Parameters 

`calendarIdentifierConstant`  

The identifier for the new calendar. For valid identifiers, see `Calendar Identifiers`.

## Return Value

The initialized calendar, or `nil` if the identifier is unknown (if, for example, it is either an unrecognized string or the calendar is not supported by the current version of the operating system).

## Discussion

The returned calendar defaults to the current locale and default time zone.

## See Also

### Related Documentation

var calendarIdentifier: NSCalendar.Identifier

An identifier for the calendar.

class var autoupdatingCurrent: Calendar

A calendar that tracks changes to user’s preferred calendar.

### Creating and Initializing Calendars

init?(calendarIdentifier: NSCalendar.Identifier)

Initializes a calendar according to a given identifier.

struct Identifier

The supported calendar types.

