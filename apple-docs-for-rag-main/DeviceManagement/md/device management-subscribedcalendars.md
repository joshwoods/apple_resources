

- Device Management
-  SubscribedCalendars 

Device Management Profile

# SubscribedCalendars

The payload you use to configure subscribed calendars.

iOS 4.0+iPadOS 4.0+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object SubscribedCalendars
```

## Properties

`SubCalAccountDescription`

`string`

The description of the account.

`SubCalAccountHostName`

`string`

 (Required) 

The server’s address.

`SubCalAccountPassword`

`string`

The user’s password.

`SubCalAccountUsername`

`string`

The user’s user name.

`SubCalAccountUseSSL`

`boolean`

If `true`, the system enables SSL.

Default: `false`

`VPNUUID`

`string`

The VPNUUID of the per-app VPN the account uses for network communication. Available in iOS 14 and later.

## Discussion

Specify `com.apple.subscribedcalendar.account` as the payload type.

### Profile Availability

|                            |                  |
|----------------------------|------------------|
| Device Channel             | iOS              |
| User Channel               | Shared iPad      |
| Allow Manual Install       | iOS              |
| Requires Supervision       | \-               |
| Requires User Approved MDM | \-               |
| Allowed in User Enrollment | iOS              |
| Allow Multiple Payloads    | iOS, Shared iPad |

### Profile Example

```

    PayloadContent

            SubCalAccountDescription
            US Holiday Calendar
            SubCalAccountHostName
            http://ical.mac.com/ical/US32Holidays.ics
            SubCalAccountUseSSL

            PayloadIdentifier
            com.example.mysubscribedcalpayload
            PayloadType
            com.apple.subscribedcalendar.account
            PayloadUUID
            c23dd040-6f68-4af2-b840-62d1943236b5
            PayloadVersion
            1

    PayloadDisplayName
    Subscribed Calendars
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    c360335c-3cfd-43d5-88c3-7e58e92821a9
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

object MobileAccounts

The payload you use to configure mobile accounts on the device.

