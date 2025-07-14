

- Device Management
-  SecurityPasskeyAttestation 

Object

# SecurityPasskeyAttestation

The declaration to configure the device to allow WebAuthn enterprise attestation for certain passkeys.

iOS 17.0+iPadOS 17.0+macOS 14.0+Device Assignment ServicesVPP License Management

``` source
object SecurityPasskeyAttestation
```

## Properties

`AttestationIdentityAssetReference`

`string`

 (Required) 

The identifier of an asset declaration that contains the identity to install and use for passkey attestation.

`AttestationIdentityKeyIsExtractable`

`boolean`

If `true`, the private key for the attestation identity is extractable in the keychain.

Default: `true`

`RelyingParties`

`[string]`

 (Required) 

An array of the relying parties to allow enterprise attestation.

## Discussion

Specify `com.apple.configuration.security.passkey.attestation` as the declaration type.

### Configuration Availability

| Allowed in Device Enrollment | iOS, macOS |
|------------------------------|------------|
| Allowed in User Enrollment   | \-         |
| Allowed in Local Enrollment  | \-         |
| Allowed in System Scope      | iOS        |
| Allowed in User Scope        | macOS      |

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

