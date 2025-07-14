

- Device Management
-  SoftwareUpdate 

Device Management Profile

# SoftwareUpdate

The payload you use to configure the software update policy.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object SoftwareUpdate
```

## Properties

`AllowPreReleaseInstallation`

`boolean`

If `true`, prerelease software can be installed on this computer.

Default: `true`

`AutomaticallyInstallAppUpdates`

`boolean`

If `false`, deselects the “Install app updates from the App Store” option and prevents the user from changing the option.

Default: `true`

`AutomaticallyInstallMacOSUpdates`

`boolean`

If `false`, restricts the “Install macOS Updates” option and prevents the user from changing the option.

Default: `true`

`AutomaticCheckEnabled`

`boolean`

If `false`, deselects the “Check for updates” option and prevents the user from changing the option.

Default: `true`

`AutomaticDownload`

`boolean`

If `false`, deselects the “Download new updates when available from the App Store” option and prevents the user from changing the option.

Default: `true`

`CatalogURL`

`string`

Deprecated 

The URL of the software update catalog. This property is not supported in macOS 11 and later.

`ConfigDataInstall`

`boolean`

If `false`, restricts the automatic installation of configuration data.

Default: `true`

`CriticalUpdateInstall`

`boolean`

If `false`, disables the automatic installation of critical updates and prevents the user from changing the “Install system data files and security updates” option.

Default: `true`

`restrict-software-update-require-admin-to-install`

`boolean`

If `true`, restrict app installations to admin users. This key has the same function as the `restrict-store-require-admin-to-install` key in the `com.apple.appstore` payload.

Default: `false`

## Discussion

Specify `com.apple.SoftwareUpdate` as the payload type.

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

            AutomaticallyInstallAppUpdates

            PayloadIdentifier
            com.example.mysoftwareupdatepayload
            PayloadType
            com.apple.SoftwareUpdate
            PayloadUUID
            af3c6efa-0dd3-4021-814b-6f2dba91428b
            PayloadVersion
            1

    PayloadDisplayName
    Software Update
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    8b6061ab-31c6-4eee-ba5b-8a09ea8f5fa7
    PayloadVersion
    1

```

## See Also

### System Updates

object SystemMigration

The payload you use to configure system migration.

