

- StoreKit
- AppStore
-  AppStore.Platform 

Structure

# AppStore.Platform

Values that represent Apple platforms.

iOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
struct Platform
```

## Discussion

You choose a platform for your app when you add the new app in App Store Connect. For more information, see Add a new app.

The platform values in `AppStore.Platform` are the same as those in App Store Connect.

## Topics

### Getting platform values

static let iOS: AppStore.Platform

A value that indicates the iOS platform.

static let macOS: AppStore.Platform

A value that indicates the macOS platform.

static let tvOS: AppStore.Platform

A value that indicates the tvOS platform.

static let visionOS: AppStore.Platform

A value that indicates the visionOS platform.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the original platform

let originalPlatform: AppStore.Platform

The platform on which the customer originally purchased the app.

