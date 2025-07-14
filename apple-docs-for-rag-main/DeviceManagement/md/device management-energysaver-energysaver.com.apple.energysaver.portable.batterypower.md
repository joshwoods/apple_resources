

- Device Management
- EnergySaver
-  EnergySaver.Com.apple.EnergySaver.portable.BatteryPower 

Device Management Profile

# EnergySaver.Com.apple.EnergySaver.portable.BatteryPower

The laptop battery power energy-saver settings.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object EnergySaver.Com.apple.EnergySaver.portable.BatteryPower
```

## Properties

`Automatic Restart On Power Loss`

`integer`

If `true`, enables “Start up automatically after a power failure.”

Possible Values: `0, 1`

`Disk Sleep Timer`

`integer`

The disk sleep time, in minutes. A value of 0 means never.

Minimum: `1`

Maximum: `180`

Value: `0`

`Display Sleep Timer`

`integer`

The display sleep time, in minutes. A value of 0 means never.

Minimum: `1`

Maximum: `180`

Value: `0`

`Dynamic Power Step`

`integer`

May not be available on all systems.

Possible Values: `0, 1`

`Reduce Processor Speed`

`integer`

May not be available on all systems.

Possible Values: `0, 1`

`System Sleep Timer`

`integer`

System sleep time, in minutes. A value of 0 means never.

Minimum: `1`

Maximum: `180`

Value: `0`

`Wake on LAN`

`integer`

If `true`, enables “Wake for network access.”

Possible Values: `0, 1`

`Wake On Modem Ring`

`integer`

If `true`, enables “Wake for modem ring.”

Possible Values: `0, 1`

## See Also

### Objects

object EnergySaver.Com.apple.EnergySaver.desktop.ACPower

The desktop AC power energy-saver settings.

object EnergySaver.Com.apple.EnergySaver.portable.ACPower

The laptop AC power energy-saver settings.

object EnergySaver.Com.apple.EnergySaver.desktop.Schedule

The schedule for turning the device on or off.

object EnergySaver.Com.apple.EnergySaver.desktop.Schedule.RepeatingPowerOff

The triggers for turning the device off.

object EnergySaver.Com.apple.EnergySaver.desktop.Schedule.RepeatingPowerOn

The triggers for turning the device on.

