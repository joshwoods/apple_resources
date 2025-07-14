

- Device Management
-  LoginWindowScripts 

Device Management Profile

# LoginWindowScripts

The payload you use to configure scripts to run at login and logout.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object LoginWindowScripts
```

## Properties

`loginscripts`

`[`LoginWindowScripts.ScriptsItems`]`

An array of one or more dictionaries of scripts to run at user login time.

`logoutscripts`

`[`LoginWindowScripts.ScriptsItems`]`

An array of one or more dictionaries of scripts to run at user logout time.

`skipLoginHook`

`boolean`

If `true`, the system doesn’t execute the login scripts during login.

Default: `false`

`skipLogoutHook`

`boolean`

If `true`, the system doesn’t execute the logout scripts during logout.

Default: `false`

## Discussion

Specify `com.apple.mcxloginscripts` as the payload type.

The MCX login and logout managed-scripts payload contains information about executable scripts that can run at user login and logout. To use this payload, set `EnableMCXLoginScripts` to `true` in `/var/root/Library/Preferences/com.apple.loginwindow.plist`; otherwise, the system ignores this payload.

`Loginwindow` uses the `LoginHook` and `LogoutHook` string keys in `/var/root/Library/Preferences/com.apple.loginwindow.plist` to indicate a path to the executable script files, which run during user login and logout. The system passes the current user name as an argument to the file.

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

            loginscripts

                    filedata
                    ExampleD
                    filename
                    ping.sh

            skipLoginHook

            skipLogoutHook

            PayloadIdentifier
            com.example.myloginwindowscriptspayload
            PayloadType
            com.apple.mcxloginscripts
            PayloadUUID
            2bcd5563-f44d-4f74-b706-050a628c0caf
            PayloadVersion
            1

    PayloadDisplayName
    Login Window Scripts
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    5cbf617d-16a5-4564-ba2c-728fd7f7d732
    PayloadVersion
    1

```

## Topics

### Objects

object LoginWindowScripts.ScriptsItems

A dictionary of login scripts.

## See Also

### Login

object LoginItemsManagedItems

The payload you use to configure a device’s login items.

object LoginWindowLoginItems

The payload you use to configure login behavior.

object LoginWindow

The payload you use to configure login window behavior.

object ServiceManagementManagedLoginItems

This payload you use to configure managed login items, which auto-enables and auto-allows matched items.

