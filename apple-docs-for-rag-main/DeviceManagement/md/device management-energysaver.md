

- Device Management
-  EnergySaver 

Device Management Profile

# EnergySaver

The payload you use to configure energy-saver settings.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object EnergySaver
```

## Properties

`com.apple.EnergySaver.desktop.ACPower`

EnergySaver.Com.apple.EnergySaver.desktop.ACPower

The settings for a desktop computer.

`com.apple.EnergySaver.desktop.Schedule`

EnergySaver.Com.apple.EnergySaver.desktop.Schedule

The schedule for turning a computer on and off.

`com.apple.EnergySaver.portable.ACPower`

EnergySaver.Com.apple.EnergySaver.portable.ACPower

The settings for a laptop computer using AC power.

`com.apple.EnergySaver.portable.BatteryPower`

EnergySaver.Com.apple.EnergySaver.portable.BatteryPower

The settings for a laptop computer using battery power.

`DestroyFVKeyOnStandby`

`boolean`

If `true`, prevents the OS from storing a temporary FileVault key in SMC or RAM for standby.

Default: `false`

`SleepDisabled`

`boolean`

If `true`, disables sleep.

Default: `false`

## Discussion

Specify `com.apple.MCX` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | macOS |

### Profile Example

```

    PayloadContent

            com.example.EnergySaver.desktop.ACPower

                Automatic Restart On Power Loss
                1
                Disk Sleep Timer
                180
                Display Sleep Timer
                60
                Sleep On Power Button
                0
                System Sleep Timer
                120
                Wake On LAN
                1

            com.apple.EnergySaver.desktop.ACPower-ProfileNumber
            -1
            com.apple.EnergySaver.desktop.Schedule

                RepeatingPowerOff

                    eventtype
                    sleep
                    time
                    0
                    weekdays
                    31

                RepeatingPowerOn

                    eventtype
                    wakepoweron
                    time
                    0
                    weekdays
                    31

            com.apple.EnergySaver.portable.ACPower

                Automatic Restart On Power Loss
                1
                Disk Sleep Timer
                180
                Display Sleep Timer
                5
                System Sleep Timer
                10
                Wake On LAN
                1

            com.apple.EnergySaver.portable.ACPower-ProfileNumber
            -1
            com.apple.EnergySaver.portable.BatteryPower

                Automatic Restart On Power Loss
                1
                Disk Sleep Timer
                180
                Display Sleep Timer
                5
                System Sleep Timer
                10
                Wake On LAN
                1

            com.apple.EnergySaver.portable.BatteryPower-ProfileNumber
            -1
            PayloadIdentifier
            com.example.myenergysaverpayload
            PayloadType
            com.apple.MCX
            PayloadUUID
            e66c94e5-f059-404e-9188-ff152cb80c64
            PayloadVersion
            1

    PayloadDisplayName
    EnergySaver
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    2627f09c-a6ea-4a2d-94b3-f6df28b3c6af
    PayloadVersion
    1

```

## Topics

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

object EnergySaver.Com.apple.EnergySaver.desktop.Schedule.RepeatingPowerOn

The triggers for turning the device on.

## See Also

### System Configuration

object Declarations

The payload to apply a set of declaration to the device through the Settings app.

object FileProvider

The payload you use to configure file provider settings.

object Font

The payload you use to configure fonts.

object LockScreenMessage

The payload you use to configure a Lock screen message.

object Screensaver

The payload you use to configure the screen saver.

object SystemExtensions

The payload you use to configure system extensions.

object SystemLogging

The payload you use to configure system logging.

object TimeServer

The payload you use to configure the time server.

