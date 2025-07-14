

- ManagedSettings
-  ManagedSettingsStore 

Class

# ManagedSettingsStore

A data store that applies settings to the current user or device.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
class ManagedSettingsStore
```

## Mentioned in 

Confirming the Effective TV and Movie Ratings

## Overview

The Managed Settings data store groups settings according to function. Each group contains relevant data about its associated settings, for example, a default value and minimum and maximum possible values.

### Configure Settings

Use the settings objects to inspect your application’s current configurations as well as apply new configurations. Changing the value of a setting to `nil` deletes your app’s configuration for that setting from the device. The system doesn’t guarantee that the settings you specify govern the device’s behavior. The system is responsible for determining its effective state based on all the settings it receives.

### Examine Effective Settings

In a few cases, you can also access the effective settings. For example, a media app can access the effective rating settings to filter the content it offers, even though it doesn’t provide configurations for these or any other settings. Subscribe to $effectiveMaximumTVShowRating or $effectiveMaximumMovieRating to determine what TV shows or movies to offer.

## Topics

### Creating the Store

init()

Creates a new instance of a store.

### Managing a Settings Group

protocol ManagedSettingsGroup

A group of settings to manage.

### Restricting Device Settings

var account: AccountSettings

Settings that affect accounts.

struct AccountSettings

An object that configures whether a user can modify their device’s account settings.

var cellular: CellularSettings

Settings that affect cellular networking.

struct CellularSettings

Constraints on the user’s cellular networking settings.

var dateAndTime: DateAndTimeSettings

Settings that affect the date and time.

struct DateAndTimeSettings

Constraints on the device’s date and time settings.

var passcode: PasscodeSettings

Settings that affect the device passcode.

struct PasscodeSettings

Constraints on a user’s ability to change their device’s passcode.

var shield: ShieldSettings

Settings that affect what activities the system covers with a shielding view on this device.

struct ShieldSettings

Constraints that indicate what apps and websites to cover with a shielding view.

var siri: SiriSettings

Settings that affect Siri.

struct SiriSettings

Constraints on the device’s Siri settings.

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

struct MediaSettings

Constraints on the media content the user can access.

### Restricting Web Content

var safari: SafariSettings

Settings that affect Safari’s search results and cookie policies.

struct SafariSettings

Constraints on Safari’s AutoFill and cookie behaviors.

var webContent: WebContentSettings

Settings that affect web content.

struct WebContentSettings

An object that configures which websites a user can access.

### Accessing Metadata

struct BoundedSettingMetadata

Additional information about a bounded setting.

struct SettingMetadata

Additional information about a configurable setting.

### Observing Current Settings

var objectWillChange: ObservableObjectPublisher

var $effectiveMaximumMovieRating: Published&lt;Int>.Publisher

The movie rating constraint that is active on this device.

var $effectiveMaximumTVShowRating: Published&lt;Int>.Publisher

The television show rating constraint that is active on this device.

typealias ObjectWillChangePublisher

The type of publisher that emits before the object has changed.

### Structures

struct Name

The unique name of a store.

### Initializers

convenience init(named: ManagedSettingsStore.Name)

Creates a new instance of a store with a custom name.

### Instance Methods

func clearAllSettings()

Clears all settings for this store.

### Default Implementations

ObservableObject Implementations

## Relationships

### Conforms To

- ObservableObject

