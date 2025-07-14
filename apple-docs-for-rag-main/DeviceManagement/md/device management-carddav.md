

- Device Management
-  CardDAV 

Device Management Profile

# CardDAV

The payload you use to configure a Contacts account.

iOS 4.0+iPadOS 4.0+macOS 10.7+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object CardDAV
```

## Properties

`CardDAVAccountDescription`

`string`

The description of the account.

`CardDAVHostName`

`string`

 (Required) 

The server’s address.

`CardDAVPassword`

`string`

The user’s password.

`CardDAVPort`

`integer`

The server’s port.

`CardDAVPrincipalURL`

`string`

The base URL to the user’s address book.

`CardDAVUsername`

`string`

The user name for logins.

`CardDAVUseSSL`

`boolean`

If `true`, the system enables SSL.

Default: `true`

`CommunicationServiceRules`

CardDAV.CommunicationServiceRules

An array of communication service rules for this account.

`VPNUUID`

`string`

The VPNUUID of the per-app VPN the account uses for network communication. Available in iOS 14 and later.

## Discussion

Specify `com.apple.carddav.account` as the payload type.

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

            CardDAVAccountDescription
            My CardDAV Account
            CardDAVHostName
            server.example.com
            CardDAVPassword
            Password123
            CardDAVPort
            443
            CardDAVUseSSL

            CardDAVUsername
            juanchavez4
            PayloadIdentifier
            com.example.mycardavpayload
            PayloadType
            com.apple.carddav.account
            PayloadUUID
            b23d14e3-2f9d-4087-a819-747903fbb176
            PayloadVersion
            1

    PayloadDisplayName
    CardDAV
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    4fdb234d-8c58-48de-a76d-9ed9d241d273
    PayloadVersion
    1

```

## Topics

### Supporting Objects

object CardDAV.CommunicationServiceRules

The communication service handler rules for this account.

## See Also

### Accounts

object Accounts

The payload you use to configure guest accounts.

object CalDAV

The payload you use to configure a Calendar account.

object GoogleAccount

The payload you use to configure a Google account.

object LDAP

The payload you use to configure an LDAP account.

object MobileAccounts

The payload you use to configure mobile accounts on the device.

object SubscribedCalendars

The payload you use to configure subscribed calendars.

