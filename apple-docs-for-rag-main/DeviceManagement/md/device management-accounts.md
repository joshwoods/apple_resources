

- Device Management
-  Accounts 

Device Management Profile

# Accounts

The payload you use to configure guest accounts.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object Accounts
```

## Properties

`DisableGuestAccount`

`boolean`

If `true`, the system disables the guest account. This property has no effect if `EnableGuestAccount` is `true`.

Default: `false`

`EnableGuestAccount`

`boolean`

If `true`, the system enables the guest account.

Default: `false`

## Discussion

Specify `com.apple.MCX` as the payload type.

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

            EnableGuestAccount

            PayloadIdentifier
            com.example.myaccountpayload
            PayloadType
            com.apple.MCX
            PayloadUUID
            5d4e377c-108c-44af-a46e-97a5aac1e270
            PayloadVersion
            1

    PayloadDisplayName
    Accounts
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    8cd28a9d-625e-4056-bbd0-43617bb8efb7
    PayloadVersion
    1

```

## See Also

### Accounts

object CalDAV

The payload you use to configure a Calendar account.

object CardDAV

The payload you use to configure a Contacts account.

object GoogleAccount

The payload you use to configure a Google account.

object LDAP

The payload you use to configure an LDAP account.

object MobileAccounts

The payload you use to configure mobile accounts on the device.

object SubscribedCalendars

The payload you use to configure subscribed calendars.

