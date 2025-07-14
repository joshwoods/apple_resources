

- ManagedSettings
-  ApplicationSettings 

Structure

# ApplicationSettings

Constraints on the apps and categories of apps a user can run on their device.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct ApplicationSettings
```

## Topics

### Blocking Applications

var blockedApplications: Set&lt;Application>?

A set of applications for the system to block.

static let blockedApplications: SettingMetadata&lt;Set&lt;Application>>

A description of the setting that controls which apps a user can launch on their device.

### Preventing App Installation and Removal

var denyAppInstallation: Bool?

A Boolean value that indicates whether to prevent the user from installing applications.

static let denyAppInstallation: SettingMetadata&lt;Bool>

The metadata for the setting to prevent app installation.

var denyAppRemoval: Bool?

A Boolean value that indicates whether to prevent the user from removing applications.

static let denyAppRemoval: SettingMetadata&lt;Bool>

The metadata for the setting to prevent app removal.

## Relationships

### Conforms To

- ManagedSettingsGroup

## See Also

### Filtering Media Content

var appStore: AppStoreSettings

Settings that affect the App Store.

struct AppStoreSettings

Constraints on a user’s App Store settings.

var application: ApplicationSettings

Settings that affect applications.

var effectiveMaximumMovieRating: Int

The movie rating constraint that is active on this device.

var effectiveMaximumTVShowRating: Int

The TV rating constraint that is active on this device.

var gameCenter: GameCenterSettings

Settings that affect Game Center.

struct GameCenterSettings

Constraints on the user’s Game Center settings.

var media: MediaSettings

Settings that affect media.

struct MediaSettings

Constraints on the media content the user can access.

