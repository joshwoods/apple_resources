

- Foundation
- TimeZone
-  timeZoneDataVersion 

Type Property

# timeZoneDataVersion

Returns the time zone data version.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var timeZoneDataVersion: String { get }
```

## See Also

### Getting Time Zone Information

var identifier: String

The geopolitical region identifier that identifies the time zone.

func abbreviation(for: Date) -> String?

Returns the abbreviation for the time zone at a given date.

func secondsFromGMT(for: Date) -> Int

The current difference in seconds between the time zone and Greenwich Mean Time.

