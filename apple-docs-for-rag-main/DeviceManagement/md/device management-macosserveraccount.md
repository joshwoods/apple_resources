

- Device Management
-  MacOSServerAccount 

Device Management Profile

# MacOSServerAccount

The payload you use to configure a macOS server account.

iOS 9.0–12.0DeprecatediPadOS 9.0–12.0DeprecatedDevice Assignment ServicesVPP License Management

``` source
object MacOSServerAccount
```

## Properties

`AccountDescription`

`string`

Deprecated 

The description of the account.

`ConfiguredAccounts`

`[`MacOSServerAccount.ConfiguredAccountsItem`]`

Deprecated   (Required) 

Array of dictionaries containing configured account types and relevant settings

`HostName`

`string`

Deprecated   (Required) 

The server’s address.

`Password`

`string`

Deprecated 

The user’s password.

`UserName`

`string`

Deprecated   (Required) 

The user’s user name.

## Discussion

Specify `com.apple.osxserver.account` as the payload type.

### Profile Availability

|                            |     |
|----------------------------|-----|
| Device Channel             | iOS |
| User Channel               | \-  |
| Allow Manual Install       | iOS |
| Requires Supervision       | \-  |
| Requires User Approved MDM | \-  |
| Allowed in User Enrollment | \-  |
| Allow Multiple Payloads    | iOS |

## Topics

### Supporting Objects

object MacOSServerAccount.ConfiguredAccountsItem

## See Also

### Deprecated

object AIMAccount

The payload you use to configure an AIM account on the device.

object APN

The payload you use to configure access point names.

object FDERecoveryKeyRedirection

The payload you use to configure FileVault recovery key redirection.

object JabberAccount

The payload you use to configure a Jabber account.

object MediaManagementAllowedMedia

The payload you use to configure media management.

object ParentalControlsDashboardWidgetRestrictions

The payload you use to configure the parental control dashboard allow list.

object ParentalControlDictationAndProfanity

The payload you use to configure parental control for dictation and profanity.

object ShareKit

The payload you use to configure ShareKit.

object SystemPreferences

The payload you use to configure the preference panes.

