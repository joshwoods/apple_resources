

- Device Management
-  MediaManagementAllowedMedia 

Device Management Profile

# MediaManagementAllowedMedia

The payload you use to configure media management.

macOS 10.7–11.0DeprecatedDevice Assignment ServicesVPP License Management

``` source
object MediaManagementAllowedMedia
```

## Properties

`logout-eject`

MediaManagementAllowedMedia.Logout-eject

Deprecated 

The media type dictionary that defines volumes to eject when the user logs out.

`mount-controls`

MediaManagementAllowedMedia.Mount-controls

Deprecated 

The media type dictionary that controls volume mounting.

`unmount-controls`

MediaManagementAllowedMedia.Unmount-controls

Deprecated 

The media type dictionary that controls volume unmounting.

## Discussion

Specify `com.apple.systemuiserver` as the payload type.

This payload is deprecated as of macOS 11.

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

object MediaManagementAllowedMedia.Logout-eject

A dictionary of volumes to eject when the user logs out.

object MediaManagementAllowedMedia.Mount-controls

A dictionary of volumes to control volume mounting.

object MediaManagementAllowedMedia.Unmount-controls

A dictionary to control volume unmounting.

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

object ParentalControlsDashboardWidgetRestrictions

The payload you use to configure the parental control dashboard allow list.

object ParentalControlDictationAndProfanity

The payload you use to configure parental control for dictation and profanity.

object ShareKit

The payload you use to configure ShareKit.

object SystemPreferences

The payload you use to configure the preference panes.

