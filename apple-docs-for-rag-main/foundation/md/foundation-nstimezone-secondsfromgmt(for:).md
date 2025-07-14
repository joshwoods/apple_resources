

- Foundation
- NSTimeZone
-  secondsFromGMT(for:) 

Instance Method

# secondsFromGMT(for:)

Returns the difference in seconds between the receiver and Greenwich Mean Time at a given date.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func secondsFromGMT(for aDate: Date) -> Int
```

## Parameters 

`aDate`  

The date against which to test the receiver.

## Return Value

The difference in seconds between the receiver and Greenwich Mean Time at `aDate`.

## Discussion

The difference may be different from the current difference if the time zone changes its offset from GMT at different points in the year—for example, the U.S. time zones change with daylight saving time.

## See Also

### Getting Time Zone Information

var name: String

The geopolitical region ID that identifies the receiver.

var abbreviation: String?

The abbreviation for the receiver, such as “EDT” (Eastern Daylight Time).

func abbreviation(for: Date) -> String?

Returns the abbreviation for the receiver at a given date.

var secondsFromGMT: Int

The current difference in seconds between the receiver and Greenwich Mean Time.

var data: Data

The data that stores the information used by the receiver.

class var timeZoneDataVersion: String

Returns the time zone data version.

enum NameStyle

Constants you use to specify a style when presenting time zone names.

