

- ManagedSettings
-  AppStoreSettings 

Structure

# AppStoreSettings

Constraints on a user’s App Store settings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct AppStoreSettings
```

## Overview

Use `AppStoreSettings` to manage a user’s App Store settings. You can set a maximum age rating for apps, deny in-app purchases, and require passwords for purchases.

## Topics

### Denying In-App Purchases

var denyInAppPurchases: Bool?

A Boolean value that indicates whether to deny the user permission to make in-app purchases.

static let denyInAppPurchases: SettingMetadata&lt;Bool>

The metadata associated with the setting to deny in-app purchases.

### Setting an App Rating Limit

var maximumRating: Int?

The maximum app rating the user can download.

static let maximumRating: BoundedSettingMetadata&lt;Int>

The metadata associated with the maximum app rating setting.

### Requiring a Password

var requirePasswordForPurchases: Bool?

A Boolean value that indicates whether to require the user’s password to make App Store transactions.

static let requirePasswordForPurchases: SettingMetadata&lt;Bool>

The metadata associated with the setting that requires a password for App Store purchases.

## Relationships

### Conforms To

- ManagedSettingsGroup

## See Also

### Filtering Media Content

var appStore: AppStoreSettings

Settings that affect the App Store.

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

struct MediaSettings

Constraints on the media content the user can access.

