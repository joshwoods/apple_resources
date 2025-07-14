

- Device Management
-  FDERecoveryKeyRedirection 

Device Management Profile

# FDERecoveryKeyRedirection

The payload you use to configure FileVault recovery key redirection.

macOS 10.9–10.13DeprecatedDevice Assignment ServicesVPP License Management

``` source
object FDERecoveryKeyRedirection
```

## Properties

`EncryptCertPayloadUUID`

`string`

Deprecated   (Required) 

The UUID of a payload within the same profile that contains a certificate used to encrypt the recovery key when it’s sent to the redirected URL. The referenced payload must be of type \`com.apple.security.pkcs1\`.

`RedirectURL`

`string`

Deprecated   (Required) 

The URL to which FDE recovery keys should be sent instead of to Apple. The URL must begin with https://.

## Discussion

Specify `com.apple.security.FDERecoveryRedirect` as the payload type.

Although the previous FDE Recovery payload is no longer supported in macOS 10.13 and later, it’s still supported in macOS 10.9 through 10.12. When installed, this payload causes any FDE recovery keys to be redirected to the specified URL instead of being sent to Apple. This requires sites to implement their own HTTPS server to receive the recovery keys through a POST request.

Note these cautions:

- The payload must exist in a system-scoped profile.

- Installing more than one payload of this type per machine results in an error.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
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

