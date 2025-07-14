

- Device Management
-  SystemLogging 

Device Management Profile

# SystemLogging

The payload you use to configure system logging.

macOS 10.12+Device Assignment ServicesVPP License Management

``` source
object SystemLogging
```

## Properties

`Subsystems`

SystemLogging.Subsystems

A dictionary enabling the logging level for subsystems. See `Customizing Logging Behavior While Debugging` for more details about the format of the dictionary.

`System`

SystemLogging.System

This dictionary has one key, `Enable-Private-Data`. Setting that value to `true` enables private data logging for the entire system.

`Processes`

SystemLogging.Processes

Not to be used.

## Discussion

Specify `com.apple.system.logging` as the payload type.

### Profile Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | macOS                                  |
| Allow Manual Install       | iOS, macOS, tvOS, watchOS              |
| Requires Supervision       | \-                                     |
| Requires User Approved MDM | \-                                     |
| Allowed in User Enrollment | \-                                     |
| Allow Multiple Payloads    | iOS, macOS, Shared iPad, tvOS, watchOS |

### Profile Example

```

    PayloadContent

            Processes

            Subsystems

                com.example.app

                    DEFAULT-OPTIONS

                        Level

                            Enable
                            Info

                        Default-Privacy-Setting
                        Public

            PayloadIdentifier
            com.example.mysystemloggingpayload
            PayloadType
            com.apple.system.logging
            PayloadUUID
            0ff59613-35e9-495c-88c8-01963de4ac80
            PayloadVersion
            1

    PayloadDisplayName
    System Logging
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    0fbfa83e-c8ec-49d0-b50c-3acc3c05749c
    PayloadVersion
    1

```

## Topics

### Objects

object SystemLogging.Processes

object SystemLogging.Subsystems

object SystemLogging.System

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

object Screensaver

The payload you use to configure the screen saver.

object SystemExtensions

The payload you use to configure system extensions.

object TimeServer

The payload you use to configure the time server.

