

- ManagedSettings
-  MediaSettings 

Structure

# MediaSettings

Constraints on the media content the user can access.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct MediaSettings
```

## Topics

### Limiting Movie and TV Show Ratings

var maximumMovieRating: Int?

The maximum movie rating the user may view.

var maximumTVShowRating: Int?

The maximum TV show rating that the user may view.

static let maximumMovieRating: BoundedSettingMetadata&lt;Int>

The metadata for the setting that controls the maximum movie rating.

static let maximumTVShowRating: BoundedSettingMetadata&lt;Int>

The metadata for the setting that controls the maximum TV show rating.

### Denying Explicit Media

var denyExplicitContent: Bool?

A Boolean value that indicates whether to prevent the user from accessing explicit content.

static let denyExplicitContent: SettingMetadata&lt;Bool>

The metadata for the setting that denies explicit content.

### Denying the Apple Music Service

var denyMusicService: Bool?

A Boolean value that indicates whether to prevent the user from accessing Apple Music’s streaming content.

static let denyMusicService: SettingMetadata&lt;Bool>

The metadata associated with denying access to Apple Music.

### Constraining Content in the Books App

var denyBookstoreErotica: Bool?

A Boolean value that indicates whether to deny media categorized as erotica in the Books store.

static let denyBookstoreErotica: SettingMetadata&lt;Bool>

The metadata associated with the setting that denies access to content in the Books store categorized as erotica.

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

struct ApplicationSettings

Constraints on the apps and categories of apps a user can run on their device.

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

