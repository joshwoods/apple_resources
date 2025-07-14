

- Device Management
-  GoogleAccount 

Device Management Profile

# GoogleAccount

The payload you use to configure a Google account.

iOS 9.3+iPadOS 9.3+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object GoogleAccount
```

## Properties

`AccountDescription`

`string`

A user-visible description of the Google account, shown in the Mail and Settings apps.

`AccountName`

`string`

The user’s full name for the Google account. This name appears in sent messages.

`CommunicationServiceRules`

GoogleAccount.CommunicationServiceRules

The communication service handler rules for this account.

`EmailAddress`

`string`

 (Required) 

The full Google email address for the account.

`VPNUUID`

`string`

The VPNUUID of the per-app VPN the account uses for network communication. Available in iOS 14 and later.

## Discussion

Specify `com.apple.google-oauth` as the payload type.

You can install multiple Google payloads. Each sets up a Google email address and any other Google services the user enables after authentication.

Note

For supervised devices, the system requires installation of Google accounts through MDM or Apple Configurator 2.

The payload never contains credentials; the system prompts the user to enter credentials shortly after installation of the payload.

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

            AccountDescription
            Google Account
            AccountName
            Juan Chavez
            EmailAddress
            juanchavez4@example.com
            PayloadIdentifier
            com.example.mygoogleaccountpayload
            PayloadType
            com.apple.google-oauth
            PayloadUUID
            0fe8f4dc-8cf0-4da3-9d5b-f734efb98a59
            PayloadVersion
            1

    PayloadDisplayName
    GoogleAccount
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    80141025-50d3-4a38-9387-ca610ff3a247
    PayloadVersion
    1

```

## Topics

### Supporting Objects

object GoogleAccount.CommunicationServiceRules

The communication service handler rules for this account.

## See Also

### Accounts

object Accounts

The payload you use to configure guest accounts.

object CalDAV

The payload you use to configure a Calendar account.

object CardDAV

The payload you use to configure a Contacts account.

object LDAP

The payload you use to configure an LDAP account.

object MobileAccounts

The payload you use to configure mobile accounts on the device.

object SubscribedCalendars

The payload you use to configure subscribed calendars.

