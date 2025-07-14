

- Foundation
- NSCalendar
-  init(calendarIdentifier:) 

Initializer

# init(calendarIdentifier:)

Initializes a calendar according to a given identifier.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(calendarIdentifier ident: NSCalendar.Identifier)
```

## Parameters 

`ident`  

The identifier for the new calendar. For valid identifiers, see `Calendar Identifiers`.

## Return Value

The initialized calendar, or `nil` if the identifier is unknown (if, for example, it is either an unrecognized string or the calendar is not supported by the current version of the operating system).

## See Also

### Related Documentation

var calendarIdentifier: NSCalendar.Identifier

An identifier for the calendar.

class var autoupdatingCurrent: Calendar

A calendar that tracks changes to user’s preferred calendar.

### Creating and Initializing Calendars

init?(identifier: NSCalendar.Identifier)

Creates a new calendar specified by a given identifier.

struct Identifier

The supported calendar types.

