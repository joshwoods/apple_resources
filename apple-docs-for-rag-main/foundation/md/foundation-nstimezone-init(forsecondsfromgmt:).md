

- Foundation
- NSTimeZone
-  init(forSecondsFromGMT:) 

Initializer

# init(forSecondsFromGMT:)

Returns a time zone object offset from Greenwich Mean Time by a given number of seconds.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(forSecondsFromGMT seconds: Int)
```

## Parameters 

`seconds`  

The number of seconds by which the new time zone is offset from GMT.

## Return Value

A time zone object offset from Greenwich Mean Time by `seconds`.

## Discussion

The name of the new time zone is GMT +/– the offset, in hours and minutes. Time zones created with this method never have daylight savings, and the offset is constant no matter the date.

## See Also

### Creating Time Zones

init?(name: String)

Returns a time zone initialized with a given identifier.

init?(name: String, data: Data?)

Initializes a time zone with a given identifier and time zone data.

convenience init?(abbreviation: String)

Returns the time zone object identified by a given abbreviation.

class var knownTimeZoneNames: [String]

Returns an array of strings listing the IDs of all the time zones known to the system.

class var abbreviationDictionary: [String : String]

Returns a dictionary holding the mappings of time zone abbreviations to time zone names.

