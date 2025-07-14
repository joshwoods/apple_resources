

- ManagedSettings
-  GameCenterSettings 

Structure

# GameCenterSettings

Constraints on the user’s Game Center settings.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct GameCenterSettings
```

## Overview

Use `GameCenterSettings` to prevent the user from changing Game Center’s settings for adding friends and joining multiplayer games.

## Topics

### Denying the Ability to Join Multiplayer Games

var denyMultiplayerGaming: Bool?

A Boolean value that indicates whether your app prevents the user joining multiplayer games.

static let denyMultiplayerGaming: SettingMetadata&lt;Bool>

The metadata associated with the setting that prevents users from joining multiplayer games.

### Denying the Ability to Add Friends

var denyAddingFriends: Bool?

A Boolean value that indicates whether to prevent the user from adding Game Center friends.

static let denyAddingFriends: SettingMetadata&lt;Bool>

The metadata for the setting that prevents the user from adding friends in Game Center.

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

var media: MediaSettings

Settings that affect media.

struct MediaSettings

Constraints on the media content the user can access.

