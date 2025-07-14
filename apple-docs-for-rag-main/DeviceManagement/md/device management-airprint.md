

- Device Management
-  AirPrint 

Device Management Profile

# AirPrint

The payload you use to configure AirPrint printers in the user’s printer list.

iOS 7.0+iPadOS 7.0+macOS 10.10+visionOS 2.0+Device Assignment ServicesVPP License Management

``` source
object AirPrint
```

## Properties

`AirPrint`

`[`AirPrint.AirPrintItem`]`

 (Required) 

An array of AirPrint printers that are presented to the user.

## Discussion

Specify `com.apple.airprint` as the payload type.

### Profile Availability

|                            |                         |
|----------------------------|-------------------------|
| Device Channel             | iOS, macOS, Shared iPad |
| User Channel               | macOS                   |
| Allow Manual Install       | iOS, macOS              |
| Requires Supervision       | \-                      |
| Requires User Approved MDM | \-                      |
| Allowed in User Enrollment | iOS                     |
| Allow Multiple Payloads    | iOS, macOS              |

### Profile Example

```

    PayloadContent

            AirPrint

                    IPAddress
                    10.0.1.42
                    ResourcePath
                    /ipp/print

            PayloadDescription
            Configures AirPrint settings
            PayloadDisplayName
            AirPrint
            PayloadIdentifier
            com.example.myairprintpayload
            PayloadType
            com.apple.airprint
            PayloadUUID
            01bd840a-42d2-4d7a-97d3-4580bc671ff9
            PayloadVersion
            1

    PayloadDisplayName
    AirPrint
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    159a5866-8323-4be1-84b1-fa4db5e04f0f
    PayloadVersion
    1

```

## Topics

### Objects

object AirPrint.AirPrintItem

A dictionary of AirPrint printer details.

## See Also

### Printing

object Printing

The payload you use to configure printers.

