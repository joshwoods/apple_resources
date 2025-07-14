

- Device Management
-  MediaManagementDiscBurning 

Device Management Profile

# MediaManagementDiscBurning

The payload you use to configure disc-burning settings.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object MediaManagementDiscBurning
```

## Properties

`BurnSupport`

`string`

 (Required) 

Configure disc-burn. Allowed values:

`off`  
The system disables disc burning.

`on`  
The system allows normal default operation. Setting this key to `on` doesn’t enable disc burn support if other mechanisms or preferences disabled it. Needs to be enabled with the Finder profile.

`authenticate`  
The system requires authentication.

Possible Values: `off, authenticate, on`

## Discussion

Specify `com.apple.DiscRecording` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            BurnSupport
            authenticate
            PayloadIdentifier
            com.example.mymediamanagementpayload
            PayloadType
            com.apple.DiscRecording
            PayloadUUID
            c7d88693-77a2-4f4d-a782-6569a1c2d92c
            PayloadVersion
            1

    PayloadDisplayName
    Media Management
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    8996588b-f785-4720-b68f-fa9c61d74bd4
    PayloadVersion
    1

```

