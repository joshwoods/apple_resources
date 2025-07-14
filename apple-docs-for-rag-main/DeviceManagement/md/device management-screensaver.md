

- Device Management
-  Screensaver 

Device Management Profile

# Screensaver

The payload you use to configure the screen saver.

macOS 10.11+Device Assignment ServicesVPP License Management

``` source
object Screensaver
```

## Properties

`askForPassword`

`boolean`

If `true`, the user is prompted for a password when the screen saver is unlocked or stopped. When you use this prompt, you must also provide `askForPasswordDelay`. Available in macOS 10.13 and later.

Default: `false`

`askForPasswordDelay`

`integer`

The number of seconds to delay before the password will be required to unlock or stop the screen saver (the grace period). A value of `2147483647` (for example, `0x7FFFFFFF`) disables this requirement. To use this option, you must set `askForPassword` to `true`. Available in macOS 10.13 and later.

`loginWindowIdleTime`

`integer`

The number of seconds of inactivity before the screen saver activates (0 = Never activate).

`loginWindowModulePath`

`string`

The full path to the screen-saver module to use.

`moduleName`

`string`

 (Required) 

The name of the screen saver module.

## Discussion

Specify `com.apple.screensaver` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            idleTime
            60
            loginWindowIdleTime
            60
            loginWindowModulePath
            /System/Library/Screen Savers/Example-Name.saver
            moduleName
            Example Name
            askForPassword

            askForPasswordDelay
            5
            PayloadIdentifier
            com.example.myscreensaverpayload
            PayloadType
            com.apple.screensaver
            PayloadUUID
            ba9abec1-ee44-413d-b75f-63748644ca71
            PayloadVersion
            1

    PayloadDisplayName
    Screem Saver Device
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    4ffe721a-f2e6-4191-a3fe-1d1a463fbbac
    PayloadVersion
    1

```

## See Also

### System Configuration

object Declarations

The payload to apply a set of declaration to the device through the Settings app.

object EnergySaver

The payload you use to configure energy-saver settings.

object FileProvider

The payload you use to configure file provider settings.

object Font

The payload you use to configure fonts.

object LockScreenMessage

The payload you use to configure a Lock screen message.

object SystemExtensions

The payload you use to configure system extensions.

object SystemLogging

The payload you use to configure system logging.

object TimeServer

The payload you use to configure the time server.

