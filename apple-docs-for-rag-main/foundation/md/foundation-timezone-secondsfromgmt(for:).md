

- Foundation
- TimeZone
-  secondsFromGMT(for:) 

Instance Method

# secondsFromGMT(for:)

The current difference in seconds between the time zone and Greenwich Mean Time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func secondsFromGMT(for date: Date = Date()) -> Int
```

## Parameters 

`date`  

The date to use for the calculation. The default value is the current date.

## See Also

### Getting Time Zone Information

var identifier: String

The geopolitical region identifier that identifies the time zone.

func abbreviation(for: Date) -> String?

Returns the abbreviation for the time zone at a given date.

static var timeZoneDataVersion: String

Returns the time zone data version.

