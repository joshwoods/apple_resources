

- Device Management
-  MobileAccounts 

Device Management Profile

# MobileAccounts

The payload you use to configure mobile accounts on the device.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object MobileAccounts
```

## Properties

`cachedaccounts.askForSecureTokenAuthBypass`

`boolean`

If `true`, the system bypasses the secure token authorization dialog. This dialog only appears on APFS volumes.

Default: `false`

`cachedaccounts.expiry.delete.disusedSeconds`

`integer`

The minimum number of seconds a mobile account can exist before the system makes an automatic attempt to remove the mobile account. Set to `0` to attempt removing it at the next login or logout. Set to `-1` to never attempt removing the mobile account.

Default: `-1`

`cachedaccounts.WarnOnCreate.allowNever`

`boolean`

If `true`, the system allows the user to stop the prompts about mobile account creation every time the user logs in. This key is only valid if `com.apple.cachedaccounts.WarnOnCreate` is `true`.

Default: `false`

`com.apple.cachedaccounts.CreateAtLogin`

`boolean`

If `true`, the system creates the mobile account at login time.

Default: `false`

`com.apple.cachedaccounts.WarnOnCreate`

`boolean`

If `true`, the system asks the user whether to create the mobile account and it allows the user to not create it.

Default: `false`

## Discussion

Specify `com.apple.MCX` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | macOS |

### Profile Example

```

    PayloadContent

            com.apple.cachedaccounts.CreateAtLogin

            PayloadIdentifier
            com.example.mymobileccountpayload
            PayloadType
            com.apple.MCX
            PayloadUUID
            93aa2058-4fe5-4f8b-a409-80f05b7fb2f0
            PayloadVersion
            1

    PayloadDisplayName
    Mobility
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    b89ce975-801b-4994-8f68-dc5cad408ad1
    PayloadVersion
    1

```

## See Also

### Accounts

object Accounts

The payload you use to configure guest accounts.

object CalDAV

The payload you use to configure a Calendar account.

object CardDAV

The payload you use to configure a Contacts account.

object GoogleAccount

The payload you use to configure a Google account.

object LDAP

The payload you use to configure an LDAP account.

object SubscribedCalendars

The payload you use to configure subscribed calendars.

