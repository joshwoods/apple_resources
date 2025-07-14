

- ManagedSettings
- Application
-  bundleIdentifier 

Instance Property

# bundleIdentifier

The unique string that identifies this app.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
let bundleIdentifier: String?
```

## Discussion

In an extension that provides shield configurations, this property provides the app’s bundle identifier. When you access this property outside that extension, the value is `nil`. See `ShieldConfigurationDataSource` in the `ManagedSettingsUI` framework for more information.

## See Also

### Accessing Application Information

let token: ApplicationToken?

An opaque representation of a specific web domain.

let localizedDisplayName: String?

A localized display name for the application.

