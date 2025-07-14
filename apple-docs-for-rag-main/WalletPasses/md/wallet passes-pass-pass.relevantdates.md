

- Wallet Passes
- Pass
-  Pass.RelevantDates 

Object

# Pass.RelevantDates

An object that represents a date interval that the system uses to show a relevant pass.

iOS 18.0+iPadOS 6.0+watchOS 2.0+

``` source
object Pass.RelevantDates
```

## Properties

`date`

`ISO 8601 date as string`

The date and time when the pass becomes relevant.

Wallet automatically calculates a relevancy interval from this date.

`endDate`

`ISO 8601 date as string`

The date and time for the pass relevancy interval to end.

Required when providing `startDate`.

`startDate`

`ISO 8601 date as string`

The date and time for the pass relevancy interval to begin.

## Discussion

Note

The values need to be a complete dates that include hours and minutes, and may optionally include seconds. For information about the ISO 8601 timestamp format, see Time and Date Formats on the W3C website.

## See Also

### Adding relevance

Showing a Pass on the Lock Screen

Add information to your pass so the system can display it on the Lock Screen at a relevant time and place.

object Pass.Locations

An object that represents a location that the system uses to show a relevant pass.

object Pass.Beacons

An object that represents the identifier of a Bluetooth Low Energy beacon the system uses to show a relevant pass.

