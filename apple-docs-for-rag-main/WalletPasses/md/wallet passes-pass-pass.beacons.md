

- Wallet Passes
- Pass
-  Pass.Beacons 

Object

# Pass.Beacons

An object that represents the identifier of a Bluetooth Low Energy beacon the system uses to show a relevant pass.

iOS 7.0+iPadOS 6.0+watchOS 2.0+

``` source
object Pass.Beacons
```

## Properties

`major`

`16-bit unsigned integer`

The major identifier of a Bluetooth Low Energy location beacon.

`minor`

`16-bit unsigned integer`

The minor identifier of a Bluetooth Low Energy location beacon.

`proximityUUID`

`string`

 (Required) 

The unique identifier of a Bluetooth Low Energy location beacon.

`relevantText`

`string`

The text to display on the lock screen when the pass is relevant. For example, a description of a nearby location, such as `“Store nearby on 1st and Main”`.

## See Also

### Adding relevance

Showing a Pass on the Lock Screen

Add information to your pass so the system can display it on the Lock Screen at a relevant time and place.

object Pass.Locations

An object that represents a location that the system uses to show a relevant pass.

object Pass.RelevantDates

An object that represents a date interval that the system uses to show a relevant pass.

