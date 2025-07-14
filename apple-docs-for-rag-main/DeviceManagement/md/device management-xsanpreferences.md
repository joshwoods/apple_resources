

- Device Management
-  XsanPreferences 

Device Management Profile

# XsanPreferences

The payload you use to configure the Xsan preferences that define the volumes that automatically mount at startup.

macOS 10.11+Device Assignment ServicesVPP License Management

``` source
object XsanPreferences
```

## Properties

`denyDLC`

`[string]`

An array of StorNext volume names. If the Xsan client is attempting to mount a volume named in this array, the client only mounts the volume if its logical units (LUNs) are available through Fibre Channel. It doesn’t attempt to mount the volume using Distributed LAN Client (DLC).

`denyMount`

`[string]`

An array of Xsan or StorNext volume names. If no `onlyMount` array is present, the Xsan client automatically attempts to mount all SAN volumes except the volumes in this array. The system administrator can mount those volumes manually by using the `xsanctl(8)` mount command.

`onlyMount`

`[string]`

An array of Xsan or StorNext volume names. The Xsan client attempts to automatically mount these volumes at startup. The system administrator can mount additional volumes manually by using the `xsanctl(8)` mount command.

`preferDLC`

`[string]`

An array of StorNext volume names. If the Xsan client is attempting to mount a volume named in this array, the Xsan client attempts to mount the volume using DLC. If DLC isn’t available, the client attempts to mount the volume if its LUNs are available through Fibre Channel. The volume name must not also appear in `denyDLC`.

`useDLC`

`boolean`

If `true`, use the DLC for all volumes.

Default: `false`

## Discussion

Specify `com.apple.xsan.preferences` as the payload type.

For more information, see https://support.apple.com/en-us/HT205333.

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

### Example Profile

```

    PayloadContent

            useDLC

            denyMount

                bob

            denyDLC

                bob

            preferDLC

                bob

            onlyMount

                bob

            PayloadIdentifier
            com.example.myxsanpreferencespayload
            PayloadType
            com.apple.xsan.preferences
            PayloadUUID
            1addfbe1-d696-4143-bec1-7cfa4121fa76
            PayloadVersion
            1

    PayloadDisplayName
    Xsan Preferences
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    63ebad99-1dbc-4b3b-a618-2789cda3eedd
    PayloadVersion
    1

```

## See Also

### Xsan

object Xsan

The payload you use to configure an Xsan client system.

