

- Device Management
-  FDEFileVaultOptions 

Device Management Profile

# FDEFileVaultOptions

The payload you use to configure FileVault options.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object FDEFileVaultOptions
```

## Properties

`DestroyFVKeyOnStandby`

`boolean`

If `true`, the system won’t store th FileVault key across restarts.

Default: `false`

`dontAllowFDEDisable`

`boolean`

If `true`, the system won’t disable FileVault.

Default: `false`

`dontAllowFDEEnable`

`boolean`

If `true`, the system won’t enable FileVault.

Default: `false`

## Discussion

Specify `com.apple.MCX` as the payload type.

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

### Profile Example

```

    PayloadContent

            dontAllowFDEDisable

            PayloadIdentifier
            com.example.myfdefvoptionspayload
            PayloadType
            com.apple.MCX
            PayloadUUID
            0a8f4102-0fbf-4d8c-b1e1-3d916f89d927
            PayloadVersion
            1

    PayloadDisplayName
    FileVault 2 Options
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    92821df0-7c04-4366-b805-eb51ed87541b
    PayloadVersion
    1

```

## See Also

### Full Disk Encryption

object FDEFileVault

The payload you use to configure FileVault.

object FDERecoveryKeyEscrow

The payload you use to configure FileVault recovery key escrow.

