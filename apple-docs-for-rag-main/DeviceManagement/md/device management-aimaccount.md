

- Device Management
-  AIMAccount 

Device Management Profile

# AIMAccount

The payload you use to configure an AIM account on the device.

macOS 10.7–10.13DeprecatedDevice Assignment ServicesVPP License Management

``` source
object AIMAccount
```

## Properties

`AIMAccountDescription`

`string`

Deprecated 

The description of the account.

`AIMAuthentication`

`string`

Deprecated   (Required) 

The authentication method for the account.

Value: `AIMAuthPassword`

`AIMHostName`

`string`

Deprecated   (Required) 

The server address.

Value: `slogin.oscar.aol.com`

`AIMPassword`

`string`

Deprecated 

The user’s password.

`AIMPort`

`integer`

Deprecated 

The connection port for the server.

Default: `5190`

Minimum: `0`

Maximum: `65535`

`AIMUserName`

`string`

Deprecated 

The user’s login name.

`AIMUseSSL`

`boolean`

Deprecated 

If `true`, enables SSL.

Default: `true`

## Discussion

Specify `com.apple.AIM.account` as the payload type.

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

object APN

The payload you use to configure access point names.

object FDERecoveryKeyRedirection

The payload you use to configure FileVault recovery key redirection.

object JabberAccount

The payload you use to configure a Jabber account.

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

