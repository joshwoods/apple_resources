

- Device Management
-  WatchEnrollment 

Object

# WatchEnrollment

The declaration to configure a Mobile Device Management v1 profile for Apple Watch enrollment.

iOS 17.0+iPadOS 17.0+Device Assignment ServicesVPP License Management

``` source
object WatchEnrollment
```

## Properties

`AnchorCertificateAssetReferences`

`[string]`

An array of identifiers of asset declarations that contain anchor certificates to use to evaluate the trust of the enrollment profile server. Set the type of the corresponding assets to `com.apple.asset.credential.certificate`.

These certificates are pinned, meaning that the server specified by the `EnrollmentProfileURL` must use a certificate that chains to one of the certs in this array.

If it chains to one of the built-in trusted root certificates but not one of the `AnchorCertificateAssetReferences` certs, the connection will fail.

`EnrollmentProfileURL`

`string`

 (Required) 

The URL of the profile that the Apple Watch downloads and installs if the user opts in to management during the pairing process, which needs to start with `https://`. Successful enrollment requires that the pairing iPhone is supervised and the profile contains an MDM payload. Apple Watch attempts to install each payload that the profile contains.

## Discussion

Specify `com.apple.configuration.watch.enrollment` as the declaration type.

### Configuration Availability

| Allowed in Device Enrollment | iOS |
|------------------------------|-----|
| Allowed in User Enrollment   | \-  |
| Allowed in Local Enrollment  | \-  |
| Allowed in System Scope      | iOS |
| Allowed in User Scope        | \-  |

## Topics

### Errors

object ErrorCodePairingTokenMissing

An error response that indicates a missing pairing token.

## See Also

### Configurations

object AccountCalDAV

The declaration to configure a Calendar account.

object AccountCardDAV

The declaration to configure an address book account.

object AccountExchange

The declaration to configure an Exchange account.

object AccountGoogle

The declaration to configure a Google account.

object AccountLDAP

The declaration to configure a Lightweight Directory Access Protocol (LDAP) account.

object AccountMail

The declaration to configure a Mail account.

object AccountSubscribedCalendar

The declaration to configure a Calendar subscription.

object AppManaged

The declaration to configure a managed app.

object DiskManagementSettings

The declaration to configure disk management settings on the device.

object LegacyInteractiveProfile

The declaration to configure an interactive, legacy profile.

object LegacyProfile

The declaration to configure a legacy profile.

object ManagementStatusSubscriptions

The declaration to configure status subscriptions.

object ManagementTest

The declaration to test the MDM system.

object MathSettings

The declaration to configure the math and calculator apps.

object PasscodeSettings

The declaration to configure passcode policy settings.

