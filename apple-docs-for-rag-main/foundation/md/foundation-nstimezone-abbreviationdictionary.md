

- Foundation
- NSTimeZone
-  abbreviationDictionary 

Type Property

# abbreviationDictionary

Returns a dictionary holding the mappings of time zone abbreviations to time zone names.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var abbreviationDictionary: [String : String] { get set }
```

## Return Value

A dictionary holding the mappings of time zone abbreviations to time zone names.

## Discussion

Note that more than one time zone may have the same abbreviation—for example, US/Pacific and Canada/Pacific both use the abbreviation “PST.” In these cases, abbreviationDictionary chooses a single name to map the abbreviation to.

## See Also

### Creating Time Zones

init?(name: String)

Returns a time zone initialized with a given identifier.

init?(name: String, data: Data?)

Initializes a time zone with a given identifier and time zone data.

convenience init?(abbreviation: String)

Returns the time zone object identified by a given abbreviation.

convenience init(forSecondsFromGMT: Int)

Returns a time zone object offset from Greenwich Mean Time by a given number of seconds.

class var knownTimeZoneNames: [String]

Returns an array of strings listing the IDs of all the time zones known to the system.

