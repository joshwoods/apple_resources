

- Device Management
-  ParentalControlsGameCenter 

Device Management Profile

# ParentalControlsGameCenter

The payload you use to configure Game Center parental controls.

macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object ParentalControlsGameCenter
```

## Properties

`GKFeatureAccountModificationAllowed`

`boolean`

If `true`, allows account modifications.

Default: `true`

`GKFeatureAddingGameCenterFriendsAllowed`

`boolean`

Deprecated 

If `true`, allows adding Game Center friends.

Default: `true`

`GKFeatureGameCenterAllowed`

`boolean`

Deprecated 

If `true`, enables Game Center.

Default: `true`

`GKFeatureMultiplayerGamingAllowed`

`boolean`

Deprecated 

If `true`, allows multiplayer gaming.

Default: `true`

## Discussion

Specify `com.apple.gamed` as the payload type.

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

            GKFeatureAccountModificationAllowed

            PayloadIdentifier
            com.example.mygamecenterpayload
            PayloadType
            com.apple.gamed
            PayloadUUID
            2967fc4d-2ab8-40db-8f3e-f6f4cfe3e408
            PayloadVersion
            1

    PayloadDisplayName
    Parental Control Game Center
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    73f89c96-6383-4db9-b879-9cc5bb8d9ad3
    PayloadVersion
    1

```

## See Also

### Parental Controls

object ParentalControlsApplicationRestrictions

The payload you use to configure parental controls for apps.

object ParentalControlsContentFilter

The payload you use to configure the parental control web content filters.

object ParentalControlsDictionary

The payload you use to configure parental control dictionary restrictions.

object ParentalControlsTimeLimits

The payload you use to configure parental control time limits.

