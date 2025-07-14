

- Device Management
- EnergySaver
- EnergySaver.Com.apple.EnergySaver.desktop.Schedule
-  EnergySaver.Com.apple.EnergySaver.desktop.Schedule.RepeatingPowerOn 

Device Management Profile

# EnergySaver.Com.apple.EnergySaver.desktop.Schedule.RepeatingPowerOn

The triggers for turning the device on.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object EnergySaver.Com.apple.EnergySaver.desktop.Schedule.RepeatingPowerOn
```

## Properties

`eventtype`

`string`

 (Required) 

The type of action defined by this schedule.

Possible Values: `wake, poweron, wakepoweron, sleep, shutdown, restart`

`time`

`integer`

The time, in minutes, since midnight.

`weekdays`

`integer`

One or more days of the week in an unsigned integer bitmap:

- `1` = Mon

- `2` = Tue

- `4` = Wed

- `8` = Thu

- `16` = Fri

- `32` = Sat

- `64` = Sun

## See Also

### Objects

object EnergySaver.Com.apple.EnergySaver.desktop.ACPower

The desktop AC power energy-saver settings.

object EnergySaver.Com.apple.EnergySaver.portable.ACPower

The laptop AC power energy-saver settings.

object EnergySaver.Com.apple.EnergySaver.portable.BatteryPower

The laptop battery power energy-saver settings.

object EnergySaver.Com.apple.EnergySaver.desktop.Schedule

The schedule for turning the device on or off.

object EnergySaver.Com.apple.EnergySaver.desktop.Schedule.RepeatingPowerOff

The triggers for turning the device off.

