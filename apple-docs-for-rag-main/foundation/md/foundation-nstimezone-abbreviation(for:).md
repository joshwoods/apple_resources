

- Foundation
- NSTimeZone
-  abbreviation(for:) 

Instance Method

# abbreviation(for:)

Returns the abbreviation for the receiver at a given date.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func abbreviation(for aDate: Date) -> String?
```

## Parameters 

`aDate`  

The date for which to get the abbreviation for the receiver.

## Return Value

The abbreviation for the receiver at `aDate`.

## Discussion

Note that the abbreviation may be different at different dates. For example, during daylight saving time the US/Eastern time zone has an abbreviation of “EDT.” At other times, its abbreviation is “EST.”

## See Also

### Getting Time Zone Information

var name: String

The geopolitical region ID that identifies the receiver.

var abbreviation: String?

The abbreviation for the receiver, such as “EDT” (Eastern Daylight Time).

var secondsFromGMT: Int

The current difference in seconds between the receiver and Greenwich Mean Time.

func secondsFromGMT(for: Date) -> Int

Returns the difference in seconds between the receiver and Greenwich Mean Time at a given date.

var data: Data

The data that stores the information used by the receiver.

class var timeZoneDataVersion: String

Returns the time zone data version.

enum NameStyle

Constants you use to specify a style when presenting time zone names.

