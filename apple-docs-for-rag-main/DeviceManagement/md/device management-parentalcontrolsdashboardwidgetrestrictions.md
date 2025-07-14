

- Device Management
-  ParentalControlsDashboardWidgetRestrictions 

Device Management Profile

# ParentalControlsDashboardWidgetRestrictions

The payload you use to configure the parental control dashboard allow list.

macOS 10.7–10.15DeprecatedDevice Assignment ServicesVPP License Management

``` source
object ParentalControlsDashboardWidgetRestrictions
```

## Properties

`WhiteList`

`[`ParentalControlsDashboardWidgetRestrictions.WhiteListItem`]`

Deprecated   (Required) 

An array of widget item dictionaries that are allowed.

`whiteListEnabled`

`boolean`

Deprecated   (Required) 

If `true`, enables the widget allow list.

## Discussion

Specify `com.apple.dashboard` as the payload type.

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

## Topics

### Objects

object ParentalControlsDashboardWidgetRestrictions.WhiteListItem

The widget item dictionary.

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

object ParentalControlDictationAndProfanity

The payload you use to configure parental control for dictation and profanity.

object ShareKit

The payload you use to configure ShareKit.

object SystemPreferences

The payload you use to configure the preference panes.

