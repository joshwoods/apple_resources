

- Foundation
- TimeZone
-  init(secondsFromGMT:) 

Initializer

# init(secondsFromGMT:)

Returns a time zone initialized with a specific number of seconds from GMT.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(secondsFromGMT seconds: Int)
```

## Parameters 

`seconds`  

The number of seconds from GMT.

## Return Value

A time zone, or `nil` if a valid time zone could not be created from `seconds`.

## Discussion

Time zones created with this never have daylight savings and the offset is constant no matter the date. The identifier and abbreviation do NOT follow the POSIX convention (of minutes-west).

## See Also

### Creating a Time Zone

static var knownTimeZoneIdentifiers: [String]

Returns an array of strings listing the identifier of all the time zones known to the system.

static var abbreviationDictionary: [String : String]

Returns the mapping of abbreviations to time zone identifiers.

