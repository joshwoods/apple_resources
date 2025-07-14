

- Foundation
- TimeZone
-  abbreviationDictionary 

Type Property

# abbreviationDictionary

Returns the mapping of abbreviations to time zone identifiers.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var abbreviationDictionary: [String : String] { get set }
```

## See Also

### Creating a Time Zone

init?(secondsFromGMT: Int)

Returns a time zone initialized with a specific number of seconds from GMT.

static var knownTimeZoneIdentifiers: [String]

Returns an array of strings listing the identifier of all the time zones known to the system.

