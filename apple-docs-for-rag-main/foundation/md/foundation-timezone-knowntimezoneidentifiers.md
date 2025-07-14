

- Foundation
- TimeZone
-  knownTimeZoneIdentifiers 

Type Property

# knownTimeZoneIdentifiers

Returns an array of strings listing the identifier of all the time zones known to the system.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var knownTimeZoneIdentifiers: [String] { get }
```

## See Also

### Creating a Time Zone

init?(secondsFromGMT: Int)

Returns a time zone initialized with a specific number of seconds from GMT.

static var abbreviationDictionary: [String : String]

Returns the mapping of abbreviations to time zone identifiers.

