

- Device Management
-  ShareKit 

Device Management Profile

# ShareKit

The payload you use to configure ShareKit.

macOS 10.9–10.12DeprecatedDevice Assignment ServicesVPP License Management

``` source
object ShareKit
```

## Properties

`SHKAllowedShareServices`

`[string]`

Deprecated 

The list of plugin IDs that show up in the user’s Share menu. If this array exists, only these items are permitted.

`SHKDeniedShareServices`

`[string]`

Deprecated 

The list of plugin IDs that won’t show up in the user’s Share menu. This key is used only if there is no `SHKAllowedShareServices` key.

## Discussion

Specify `com.apple.ShareKitHelper` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

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

object MacOSServerAccount

The payload you use to configure a macOS server account.

object MediaManagementAllowedMedia

The payload you use to configure media management.

object ParentalControlsDashboardWidgetRestrictions

The payload you use to configure the parental control dashboard allow list.

object ParentalControlDictationAndProfanity

The payload you use to configure parental control for dictation and profanity.

object SystemPreferences

The payload you use to configure the preference panes.

