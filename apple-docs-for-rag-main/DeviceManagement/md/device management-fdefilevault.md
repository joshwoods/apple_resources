

- Device Management
-  FDEFileVault 

Device Management Profile

# FDEFileVault

The payload you use to configure FileVault.

macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object FDEFileVault
```

## Properties

`Certificate`

`data`

The DER-encoded certificate data if the system creates an institutional recovery key. This key isn’t supported on Macs with Apple silicon.

`Defer`

`boolean`

If `true`, the system defers enabling FileVault until the designated user logs out. For details, see `fdesetup(8)`. Only a local user or a mobile account user can enable FileVault.

Default: `false`

`DeferDontAskAtUserLogout`

`boolean`

If `true`, the system prevents requests to enable FileVault at user logout time.

Default: `false`

`DeferForceAtUserLoginMaxBypassAttempts`

`integer`

The maximum number of times users can bypass enabling FileVault before the system requires the user to enable it to log in. If the value is `0`, the system requires the user to enable FileVault the next time they attempt to log in. Set this key to `-1` to disable this feature.

Minimum: `-1`

Maximum: `9999`

`Enable`

`string`

 (Required) 

Set to `On` to enable FileVault and set to `Off` to disable FileVault. Payloads set to `On` sent through MDM need to either include full authentication information in the payload or have the `Defer` option set to `true`. When `Defer` is `true`, the system prompts for the authentication information when the user enables FileVault.

Possible Values: `On, Off`

`ForceEnableInSetupAssistant`

`boolean`

If `true`, and installation of this payload occurs after enrolling with MDM in Setup Assistant, the system requests Setup Assistant to enable FileVault at setup time.

To use this, enable the Await Device Configured DEP configuration option and send this profile with this key set, before sending the DeviceConfiguredCommand.

Default: `false`

`OutputPath`

`string`

The path to the location of the recovery key and computer information property list.

`Password`

`string`

The password of the Open Directory user to add to FileVault. Use the `UserEntersMissingInfo` key to prompt for this information.

`PayloadCertificateUUID`

`string`

The UUID of the payload within the same profile containing the asymmetric recovery key certificate payload.

`ShowRecoveryKey`

`boolean`

If `false`, the system prevents display of the personal recovery key to the user after the system enables FileVault.

Default: `true`

`UseKeychain`

`boolean`

If `true` and you don’t include certificate information in this payload, the system uses the keychain created at `/Library/Keychains/FileVaultMaster.keychain` when it adds the institutional recovery key.

Default: `false`

`UseRecoveryKey`

`boolean`

If `true`, the system creates a personal recovery key and displays it to the user.

Default: `true`

`UserEntersMissingInfo`

`boolean`

If `true`, the system enables a prompt for missing user name or password fields.

Default: `false`

`Username`

`string`

The user name of the Open Directory user to add to FileVault.

## Discussion

Specify `com.apple.MCX.FileVault2` as the payload type.

FileVault 2 performs full XTS-AES 128 encryption on the contents of a volume. Removing the FileVault payload doesn’t disable FileVault.

As of macOS 10.15, FileVault settings require supervision or user approval when installed manually.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | macOS |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            Defer

            Enable
            On
            ShowRecoveryKey

            UseKeychain

            UseRecoveryKey

            UserEntersMissingInfo

            PayloadIdentifier
            com.example.myfdefilevaultpayload
            PayloadType
            com.apple.MCX.FileVault2
            PayloadUUID
            c2c5f5e9-8ffc-4d8f-9108-fd655b90fdb2
            PayloadVersion
            1

    PayloadDisplayName
    FDE File Vault
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    5ba0de0e-ff06-4c0b-8dca-f5b55ed9de86
    PayloadVersion
    1

```

## See Also

### Full Disk Encryption

object FDEFileVaultOptions

The payload you use to configure FileVault options.

object FDERecoveryKeyEscrow

The payload you use to configure FileVault recovery key escrow.

