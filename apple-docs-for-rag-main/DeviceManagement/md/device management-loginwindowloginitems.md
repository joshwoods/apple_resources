

- Device Management
-  LoginWindowLoginItems 

Device Management Profile

# LoginWindowLoginItems

The payload you use to configure login behavior.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object LoginWindowLoginItems
```

## Properties

`DisableLoginItemsSuppression`

`boolean`

If `true`, the system prevents the user from disabling login item launches by using the Shift key.

Default: `false`

## Discussion

Specify `loginwindow` as the payload type.

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

            DisableLoginItemsSuppression

            PayloadIdentifier
            com.example.myloginwindowloginitemspayload
            PayloadType
            loginwindow
            PayloadUUID
            e032844e-db81-4387-98d9-9ee7c6038275
            PayloadVersion
            1

    PayloadDisplayName
    Login Window Login Items
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    30724e47-e58e-447d-b21c-a65bbe184f98
    PayloadVersion
    1

```

## See Also

### Login

object LoginItemsManagedItems

The payload you use to configure a device’s login items.

object LoginWindow

The payload you use to configure login window behavior.

object LoginWindowScripts

The payload you use to configure scripts to run at login and logout.

object ServiceManagementManagedLoginItems

This payload you use to configure managed login items, which auto-enables and auto-allows matched items.

