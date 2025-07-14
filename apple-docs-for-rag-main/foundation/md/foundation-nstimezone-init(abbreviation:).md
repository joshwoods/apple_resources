

- Foundation
- NSTimeZone
-  init(abbreviation:) 

Initializer

# init(abbreviation:)

Returns the time zone object identified by a given abbreviation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init?(abbreviation: String)
```

## Parameters 

`abbreviation`  

An abbreviation for a time zone.

## Return Value

The time zone object identified by `abbreviation` determined by resolving the abbreviation to a name using the abbreviation dictionary and then returning the time zone for that name. Returns `nil` if there is no match for `abbreviation`.

## Discussion

In general, you are discouraged from using abbreviations except for unique instances such as “GMT”. Time Zone abbreviations are not standardized and so a given abbreviation may have multiple meanings—for example, “EST” refers to Eastern Time in both the United States and Australia

## See Also

### Related Documentation

Date and Time Programming Guide

### Creating Time Zones

init?(name: String)

Returns a time zone initialized with a given identifier.

init?(name: String, data: Data?)

Initializes a time zone with a given identifier and time zone data.

convenience init(forSecondsFromGMT: Int)

Returns a time zone object offset from Greenwich Mean Time by a given number of seconds.

class var knownTimeZoneNames: [String]

Returns an array of strings listing the IDs of all the time zones known to the system.

class var abbreviationDictionary: [String : String]

Returns a dictionary holding the mappings of time zone abbreviations to time zone names.

