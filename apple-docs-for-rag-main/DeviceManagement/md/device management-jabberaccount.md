

- Device Management
-  JabberAccount 

Device Management Profile

# JabberAccount

The payload you use to configure a Jabber account.

macOS 10.7–10.14DeprecatedDevice Assignment ServicesVPP License Management

``` source
object JabberAccount
```

## Properties

`JabberAccountDescription`

`string`

Deprecated 

The description of the account.

`JabberAuthentication`

`string`

Deprecated   (Required) 

The authentication method for the account.

Value: `JabberAuthPassword`

`JabberHostName`

`string`

Deprecated   (Required) 

The server’s address.

`JabberPassword`

`string`

Deprecated 

The user’s password.

`JabberPort`

`integer`

Deprecated 

The server’s port.

Default: `5222`

Minimum: `0`

Maximum: `65535`

`JabberUserName`

`string`

Deprecated 

The user’s user name.

`JabberUseSSL`

`boolean`

Deprecated 

If `true`, enables SSL.

Default: `false`

## Discussion

Specify `com.apple.jabber.account` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | \-    |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | macOS |

## See Also

### Deprecated

object AIMAccount

The payload you use to configure an AIM account on the device.

object APN

The payload you use to configure access point names.

object FDERecoveryKeyRedirection

The payload you use to configure FileVault recovery key redirection.

object MacOSServerAccount

The payload you use to configure a macOS server account.

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

