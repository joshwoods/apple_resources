

- Device Management
-  LoginWindow 

Device Management Profile

# LoginWindow

The payload you use to configure login window behavior.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object LoginWindow
```

## Properties

`AdminHostInfo`

`string`

The admin host info. If present in the payload, the system displays its value in the login window as additional computer information. Before macOS 10.10, this string could only contain host name, system version, or IP address. After macOS 10.10, setting this key to any value allows the user to click the time area of the menu bar to toggle through various computer information values.

Possible Values: `HostName, SystemVersion, IPAddress`

`AllowList`

`[string]`

The list of user GUIDs or group GUIDs of users that the system allows to log in. An asterisk (`*`) string specifies all users or groups.

`AutologinPassword`

`string`

An optional user password to set up auto login. If this key doesn’t exist but a user name does exist, the system sets up auto login the next time the user logs in to the client.

`AutologinUsername`

`string`

The user short name to set up auto login.

`DenyList`

`[string]`

The list of user GUIDs or group GUIDs of users that the system disallows to log in. This list takes priority over the list in the `AllowList` key.

`DisableConsoleAccess`

`boolean`

If `true`, the system disregards the `>console` special user name, which provides a command line UI.

Default: `false`

`DisableFDEAutoLogin`

`boolean`

If t`rue`, the system disables the automatic login option when using FileVault.

Default: `false`

`DisableScreenLockImmediate`

`boolean`

If `true`, the system disables the immediate Screen Lock functions. Available in macOS 10.13 and later.

Default: `false`

`HideAdminUsers`

`boolean`

If `true`, the system hides administrator users when showing a user list.

Default: `false`

`HideLocalUsers`

`boolean`

If `true`, the system shows only network and system users when showing a user list.

Default: `false`

`HideMobileAccounts`

`boolean`

If `true`, the system hides mobile account users in a user list. In some cases, mobile users show up as network users.

Default: `false`

`IncludeNetworkUser`

`boolean`

If `true`, the system shows network users when showing a user list.

Default: `false`

`LoginwindowText`

`string`

The text to display in the login window.

`LogOutDisabledWhileLoggedIn`

`boolean`

If `true`, the system disables the Log Out menu item when the user is logged in. Available in macOS 10.13 and later.

Default: `false`

`PowerOffDisabledWhileLoggedIn`

`boolean`

If `true`, the system disables the Power Off menu item when the user is logged in.

Default: `false`

`RestartDisabled`

`boolean`

If `true`, the system disables the Restart item.

Default: `false`

`RestartDisabledWhileLoggedIn`

`boolean`

If `true`, the system disables the Restart menu item when the user is logged in.

Default: `false`

`SHOWFULLNAME`

`boolean`

If `true`, the system shows the name and password dialog. If `false`, the system displays a list of users.

Default: `false`

`SHOWOTHERUSERS_MANAGED`

`boolean`

If `true`, the system displays “Other…” when it shows a list of users.

Default: `false`

`showInputMenu`

`boolean`

If `true`, the system shows the Input Menu in the login window.

Default: `false`

`ShutDownDisabled`

`boolean`

If `true`, the system disables the Shut Down button.

Default: `false`

`SleepDisabled`

`boolean`

If `true`, the system disables the Sleep button.

Default: `false`

`ShutDownDisabledWhileLoggedIn`

`boolean`

If `true`, the system disables the Shut Down menu item when the user is logged in.

Default: `false`

## Discussion

Specify `com.apple.loginwindow` as the payload type.

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

            AdminHostInfo
            HostName
            AdminMayDisableMCX

            AllowList

            AlwaysShowWorkgroupDialog

            CombineUserWorkgroups

            DenyList

            DisableConsoleAccess

            EnableExternalAccounts

            FlattenUserWorkgroups

            HideAdminUsers

            HideLocalUsers

            HideMobileAccounts

            IncludeNetworkUser

            LocalUserLoginEnabled

            LocalUsersHaveWorkgroups

            RestartDisabled

            RetriesUntilHint
            0
            SHOWFULLNAME

            SHOWOTHERUSERS_MANAGED

            ShutDownDisabled

            SleepDisabled

            UseComputerNameForComputerRecordName

            com.apple.login.mcx.DisableAutoLoginClient

            showInputMenu

            PayloadIdentifier
            com.example.myloginwindowpayload
            PayloadType
            com.apple.loginwindow
            PayloadUUID
            fe9ba3c5-0f1a-45c7-b6df-a5f4489695fe
            PayloadVersion
            1

    PayloadDisplayName
    Login Window
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    61bd7d63-4a4a-4b67-9112-5ceb16afb4dc
    PayloadVersion
    1

```

## See Also

### Login

object LoginItemsManagedItems

The payload you use to configure a device’s login items.

object LoginWindowLoginItems

The payload you use to configure login behavior.

object LoginWindowScripts

The payload you use to configure scripts to run at login and logout.

object ServiceManagementManagedLoginItems

This payload you use to configure managed login items, which auto-enables and auto-allows matched items.

