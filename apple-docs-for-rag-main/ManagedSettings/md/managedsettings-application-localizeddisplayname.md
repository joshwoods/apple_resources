

- ManagedSettings
- Application
-  localizedDisplayName 

Instance Property

# localizedDisplayName

A localized display name for the application.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
let localizedDisplayName: String?
```

## Discussion

In an extension that provides shield configurations, this property provides the app’s name. When you access this property outside that extension, the value is `nil`. See `ShieldConfigurationDataSource` in the Managed Settings UI framework for more information.

## See Also

### Accessing Application Information

let bundleIdentifier: String?

The unique string that identifies this app.

let token: ApplicationToken?

An opaque representation of a specific web domain.

