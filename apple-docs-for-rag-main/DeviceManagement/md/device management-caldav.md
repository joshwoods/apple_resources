

- Device Management
-  CalDAV 

Device Management Profile

# CalDAV

The payload you use to configure a Calendar account.

iOS 4.0+iPadOS 4.0+macOS 10.7+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object CalDAV
```

## Properties

`CalDAVAccountDescription`

`string`

The description of the account.

`CalDAVHostName`

`string`

 (Required) 

The server’s address.

`CalDAVPassword`

`string`

The user’s password. The system only uses this with encrypted profiles.

`CalDAVPort`

`integer`

The server’s port.

`CalDAVPrincipalURL`

`string`

The base URL to the user’s calendar.

`CalDAVUsername`

`string`

The user name for logins. If this profile is part of a non-interactive install, the system requires this field.

`CalDAVUseSSL`

`boolean`

If `true`, the system enables SSL.

Default: `true`

`VPNUUID`

`string`

The VPNUUID of the per-app VPN the account uses for network communication. Available in iOS 14 and later.

## Discussion

Specify `com.apple.caldav.account` as the payload type.

### Profile Availability

|                            |                         |
|----------------------------|-------------------------|
| Device Channel             | iOS                     |
| User Channel               | macOS, Shared iPad      |
| Allow Manual Install       | iOS, macOS              |
| Requires Supervision       | \-                      |
| Requires User Approved MDM | \-                      |
| Allowed in User Enrollment | iOS, macOS              |
| Allow Multiple Payloads    | iOS, macOS, Shared iPad |

### Profile Example

```

    PayloadContent

            CalDAVAccountDescription
            My CalDAV Account
            CalDAVHostName
            server.example.com
            CalDAVPassword
            Password123
            CalDAVPort
            443
            CalDAVUseSSL

            CalDAVUsername
            juanchavez4@example.com
            PayloadIdentifier
            com.example.mycaldavpayload
            PayloadType
            com.apple.caldav.account
            PayloadUUID
            603409f1-b611-459d-9584-0ed12bc25b5b
            PayloadVersion
            1

    PayloadDisplayName
    CalDAV
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    5c8bb406-a74c-4338-93c6-b403a040cc91
    PayloadVersion
    1

```

## See Also

### Accounts

object Accounts

The payload you use to configure guest accounts.

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

