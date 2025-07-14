

- ManagedSettings
- ApplicationSettings
-  denyAppRemoval 

Type Property

# denyAppRemoval

The metadata for the setting to prevent app removal.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static let denyAppRemoval: SettingMetadata
```

## Discussion

Use `denyAppRemoval` to access metadata about denyAppRemoval. The default value is `false`.

## See Also

### Preventing App Installation and Removal

var denyAppInstallation: Bool?

A Boolean value that indicates whether to prevent the user from installing applications.

static let denyAppInstallation: SettingMetadata&lt;Bool>

The metadata for the setting to prevent app installation.

var denyAppRemoval: Bool?

A Boolean value that indicates whether to prevent the user from removing applications.

