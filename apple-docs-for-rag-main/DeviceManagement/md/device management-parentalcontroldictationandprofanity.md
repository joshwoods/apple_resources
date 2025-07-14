

- Device Management
-  ParentalControlDictationAndProfanity 

Device Management Profile

# ParentalControlDictationAndProfanity

The payload you use to configure parental control for dictation and profanity.

macOS 10.9–10.13DeprecatedDevice Assignment ServicesVPP License Management

``` source
object ParentalControlDictationAndProfanity
```

## Properties

`Ironwood Allowed`

`boolean`

Deprecated 

If `false`, disables dictation. Use `allowDictation` in Restrictions instead.

Default: `true`

`Profanity Allowed`

`boolean`

Deprecated 

If `false`, suppresses profanity. Use `forceAssistantProfanityFilter` in Restrictions instead.

Default: `true`

## Discussion

Specify `com.apple.ironwood.support` as the payload type.

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

object ShareKit

The payload you use to configure ShareKit.

object SystemPreferences

The payload you use to configure the preference panes.

