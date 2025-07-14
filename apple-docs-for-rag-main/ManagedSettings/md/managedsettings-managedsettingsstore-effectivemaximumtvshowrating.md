

- ManagedSettings
- ManagedSettingsStore
-  effectiveMaximumTVShowRating 

Instance Property

# effectiveMaximumTVShowRating

The TV rating constraint that is active on this device.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@Published
var effectiveMaximumTVShowRating: Int { get }
```

## Mentioned in 

Confirming the Effective TV and Movie Ratings

## Discussion

An authorized app can use the Family Controls framework to apply a maximumTVShowRating to the device. If no `maximumTVShowRating` settings are active, then the value of this property is the default value of maximumTVShowRating. The system publishes changes dynamically.

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

var gameCenter: GameCenterSettings

Settings that affect Game Center.

struct GameCenterSettings

Constraints on the user’s Game Center settings.

var media: MediaSettings

Settings that affect media.

struct MediaSettings

Constraints on the media content the user can access.

