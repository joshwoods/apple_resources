

- ManagedSettings
- ApplicationSettings
-  denyAppInstallation 

Type Property

# denyAppInstallation

The metadata for the setting to prevent app installation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static let denyAppInstallation: SettingMetadata
```

## Discussion

Use `denyAppInstallation` to access metadata about denyAppInstallation. The default value is `false`.

## See Also

### Preventing App Installation and Removal

var denyAppInstallation: Bool?

A Boolean value that indicates whether to prevent the user from installing applications.

var denyAppRemoval: Bool?

A Boolean value that indicates whether to prevent the user from removing applications.

static let denyAppRemoval: SettingMetadata&lt;Bool>

The metadata for the setting to prevent app removal.

