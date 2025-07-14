

- MarketplaceKit
-  AppLibrary 

Class

# AppLibrary

An object that manages search characteristics, licensing, and the installation of apps.

iOS 17.4+iPadOS 17.4+

``` source
@MainActor
final class AppLibrary
```

## Mentioned in 

Supplying an install verification token

Installing apps from an alternative marketplace

## Overview

Alternative app marketplaces call methods of this class to request the installation of iOS apps from within their app, or to update the license for a specific app that the marketplace distributes. In addition, web browsers that render with BrowserEngineKit rather than WebKit call a method of this class to implement the installation of alternative app marketplaces from a webpage. You can also customize Spotlight search results for the detail using the setSearchTerritory(_:) method.

iOS ignores calls to this class for apps that lack one of the required entitlements:

- com.apple.developer.marketplace.app-installation

- com.apple.developer.browser.app-installation

## Topics

### Filtering app searches

var searchTerritory: String?

A country code that iOS uses to filter the search results of apps that aren’t available in that country.

func setSearchTerritory(String?) async

Defines a country code that iOS uses to filter the search results of apps that aren’t available in that country.

### Classes

class App

Information about an app that someone installs from a marketplace, including its ID and installation status.

### Structures

struct InstallationRequest

### Instance Properties

var installedApps: Set&lt;AppLibrary.App>

var installingApps: Set&lt;AppLibrary.App>

var isLoading: Bool

### Instance Methods

func app(forAppleItemID: AppleItemID) -> AppLibrary.App

func didAuthenticate(account: String) async

Instructs iOS to reinstall an app after a required reuthorization completes.

func requestAppInstallation(AppLibrary.InstallationRequest) async throws

func requestAppInstallation(for: URL, account: String, installVerificationToken: String) async throwsDeprecated

func requestAppInstallationFromBrowser(for: URL, referrer: URL) async throws

Forwards an app installation request from the developer’s webpage.

func requestAppUpdate(AppLibrary.InstallationRequest) async throws

func requestAppUpdate(for: URL, account: String, installVerificationToken: String) async throwsDeprecated

func requestLicenseRenewal(appleItemIDs: [UInt64]) async throws

Instructs iOS to request an updated app license from your marketplace server for the given app identifier.

### Type Properties

static let current: AppLibrary

## Relationships

### Conforms To

- Copyable
- Observable
- Sendable

## See Also

### App management

struct AppVersion

Information that describes an app, including its identifier and version number.

struct AutomaticUpdate

Information that describes an app that’s available for update, including a download URL.

struct InstallRequirements

An app’s installation criteria for a device.

typealias AppleItemID

An identifier that represents an app.

typealias AppleVersionID

An identifier that represents a single app version.

let MarketplaceKitURIScheme: String

A URI scheme that defines an alternative distribution app installation link.

