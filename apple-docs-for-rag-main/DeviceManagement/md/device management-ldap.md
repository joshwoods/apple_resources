

- Device Management
-  LDAP 

Device Management Profile

# LDAP

The payload you use to configure an LDAP account.

iOS 4.0+iPadOS 4.0+macOS 10.7+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object LDAP
```

## Properties

`LDAPAccountDescription`

`string`

The description of the account.

`LDAPAccountHostName`

`string`

 (Required) 

The server’s address.

`LDAPAccountPassword`

`string`

The user’s password. The system only enables the password with encrypted profiles.

`LDAPAccountUserName`

`string`

The user’s user name.

`LDAPAccountUseSSL`

`boolean`

If `true`, the system enables SSL.

Default: `true`

`LDAPSearchSettings`

`[`LDAP.LDAPSearchSettingsItem`]`

An array of search settings dictionaries.

`VPNUUID`

`string`

The VPNUUID of the per-app VPN the account uses for network communication. Available in iOS 14 and later.

## Discussion

Specify `com.apple.ldap.account` as the payload type.

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

            LDAPAccountDescription
            Company LDAP Account
            LDAPAccountHostName
            com.apple.ldap.account
            LDAPAccountUseSSL

            LDAPAccountUserName
            JuanChavez4
            LDAPSearchSettings

                    LDAPSearchSettingDescription
                    My Search
                    LDAPSearchSettingScope
                    LDAPSearchSettingScopeSubtree
                    LDAPSearchSettingSearchBase
                    o=My Company,ou=My Department

            PayloadIdentifier
            com.example.myldappayload
            PayloadType
            com.apple.ldap.account
            PayloadUUID
            7f846724-1bf7-4501-b8cd-ce7026e95280
            PayloadVersion
            1

    PayloadDisplayName
    LDAP
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    c5208028-7e96-4669-8d83-4fbbeb48845a
    PayloadVersion
    1

```

## Topics

### Supporting Objects

object LDAP.LDAPSearchSettingsItem

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

object MobileAccounts

The payload you use to configure mobile accounts on the device.

object SubscribedCalendars

The payload you use to configure subscribed calendars.

