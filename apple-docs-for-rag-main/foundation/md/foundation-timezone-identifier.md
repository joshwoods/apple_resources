

- Foundation
- TimeZone
-  identifier 

Instance Property

# identifier

The geopolitical region identifier that identifies the time zone.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var identifier: String { get }
```

## See Also

### Getting Time Zone Information

func abbreviation(for: Date) -> String?

Returns the abbreviation for the time zone at a given date.

func secondsFromGMT(for: Date) -> Int

The current difference in seconds between the time zone and Greenwich Mean Time.

static var timeZoneDataVersion: String

Returns the time zone data version.

