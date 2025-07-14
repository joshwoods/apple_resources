

- MarketplaceKit
-  MarketplaceExtension 

Protocol

# MarketplaceExtension

An extension that facilitates authentication, installation, and launching a marketplace with deep links.

iOS 17.4+iPadOS 17.4+

``` source
protocol MarketplaceExtension : AppExtension, Sendable
```

## Mentioned in 

Installing apps from an alternative marketplace

Reauthenticating a person to manage apps

## Overview

You provide this extension to enable the operating system to facilitate some tasks for your app even if it isn’t running, such as:

- Automatically updating apps when a new version is available.

- Provide additional header text for communications with your marketplace server.

- Launching your app storefront for a specific app.

- Handling failures in requests to your marketplace server.

### Define the extension point identifier

To set up your marketplace extension in Xcode, use a generic extension template and set the `EXExtensionPointIdentifier` `Info.plist` key to `com.apple.marketplace.extension`:

```

  EXAppExtensionAttributes

    EXExtensionPointIdentifier
    com.apple.marketplace.extension

```

## Topics

### Instance Methods

func additionalHeaders(for: URLRequest, account: String) -> [String : String]?

Adds information to the request header for communications from the operating system to your marketplace endpoints.

**Required**

func automaticUpdates(for: [AppVersion]) async throws -> [AutomaticUpdate]

**Required**

func availableAppVersions(forAppleItemIDs: [AppleItemID]) -> [AppVersion]?

**Required**

func requestFailed(with: HTTPURLResponse) -> Bool

Handles when iOS receives an unexpected response from your web server.

**Required**

## Relationships

### Inherits From

- AppExtension
- Sendable

## See Also

### Background services

protocol MarketplaceExtensionConfiguration

The type for a marketplace extension’s configuration object.

