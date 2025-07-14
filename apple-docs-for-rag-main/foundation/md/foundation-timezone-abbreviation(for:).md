

- Foundation
- TimeZone
-  abbreviation(for:) 

Instance Method

# abbreviation(for:)

Returns the abbreviation for the time zone at a given date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func abbreviation(for date: Date = Date()) -> String?
```

## Parameters 

`date`  

The date to use for the calculation. The default value is the current date.

## Discussion

Note that the abbreviation may be different at different dates. For example, during daylight saving time the US/Eastern time zone has an abbreviation of “EDT.” At other times, its abbreviation is “EST.”

## See Also

### Getting Time Zone Information

var identifier: String

The geopolitical region identifier that identifies the time zone.

func secondsFromGMT(for: Date) -> Int

The current difference in seconds between the time zone and Greenwich Mean Time.

static var timeZoneDataVersion: String

Returns the time zone data version.

